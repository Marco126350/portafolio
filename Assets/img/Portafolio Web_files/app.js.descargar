// **********TOGGLE ICONS NAVBAR*********
let menuIcon = document.querySelector('#menu-icon');
let navbar = document.querySelector('.header__navbar');

menuIcon.onclick = () => {
  menuIcon.classList.toggle('fa-x');
  navbar.classList.toggle('acto');
}

// **********SCROLL SECTIONS ACTIVE LINK*********
let sections = document.querySelectorAll('section');
let navLinks = document.querySelectorAll('header nav a');

window.onscroll = () => {
  sections.forEach(sec => {
    let top = window.scrollY;
    let offset = sec.offsetTop - 150;
    let height = sec.offsetHeight;
    let id = sec.getAttribute('id');

    if (top >= offset && top < offset + height) {
      navLinks.forEach(links => {
        links.classList.remove('active');
        document.querySelector('header nav a[href*=' + id + ']').classList.add('active');
      });
    };
  });

  // **********STICKY NAVBAR*********
  // let header = document.querySelector('header');
  
  // header.classList.toggle('sticky', window.scrollY > 100);

  // **********REMOVE TOGGLE ICON AND NAVBAR WHEN CLICK NAVVBAR LINK(SCROLL)*********
 
  navbar.onclick = () => {
  menuIcon.classList.remove('fa-x');
  navbar.classList.remove('acto');
  }

};

 // **********SCROLL REVEAL*********
 ScrollReveal({
   // reset: true,
   distance: '80px',
   duration: 2000,
   delay: 200
  });
  
  ScrollReveal().reveal('.home__hero-image-content, .heading', { origin:'top' });
  ScrollReveal().reveal('.home-img, .portfolio__container-box', { origin:'bottom' });
  ScrollReveal().reveal('.home__hero-image-content h1,.services__container-box',  { origin:'left' });
  ScrollReveal().reveal('.home__hero-image-content p, .about__content', { origin: 'right' });
  
  
  // **********TYPED JS*********
const typed = new Typed('.multiple-text', {
  strings: ['Software Engineer '],
  typeSpeed: 100,
  backSpeed: 100,
  backDelay: 1000,

  })