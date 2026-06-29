/* ==========================================
   TREY MAVRIK OFFICIAL WEBSITE
   script.js
========================================== */

/* Smooth fade-in animation */

const sections = document.querySelectorAll("section");

const observer = new IntersectionObserver((entries) => {

entries.forEach((entry)=>{

if(entry.isIntersecting){

entry.target.style.opacity="1";
entry.target.style.transform="translateY(0)";

}

});

},{
threshold:0.15
});

sections.forEach((section)=>{

section.style.opacity="0";
section.style.transform="translateY(60px)";
section.style.transition="all 0.9s ease";

observer.observe(section);

});


/* Navbar shadow while scrolling */

const navbar=document.querySelector(".navbar");

window.addEventListener("scroll",()=>{

if(window.scrollY>80){

navbar.style.background="#000";
navbar.style.boxShadow="0 10px 35px rgba(0,0,0,.5)";

}else{

navbar.style.background="rgba(0,0,0,.85)";
navbar.style.boxShadow="none";

}

});


/* Active navigation */

const navLinks=document.querySelectorAll(".navbar a");

navLinks.forEach(link=>{

link.addEventListener("click",()=>{

navLinks.forEach(item=>{

item.classList.remove("active");

});

link.classList.add("active");

});

});


/* Button hover effect */

const buttons=document.querySelectorAll("a");

buttons.forEach(button=>{

button.addEventListener("mouseenter",()=>{

button.style.transform="translateY(-5px)";

});

button.addEventListener("mouseleave",()=>{

button.style.transform="translateY(0)";

});

});


/* Album card animation */

const albums=document.querySelectorAll(".album-card");

albums.forEach(card=>{

card.addEventListener("mouseenter",()=>{

card.style.transform="translateY(-10px) scale(1.02)";

});

card.addEventListener("mouseleave",()=>{

card.style.transform="translateY(0) scale(1)";

});

});


/* Newsletter */

const form=document.querySelector(".newsletter form");

if(form){

form.addEventListener("submit",(e)=>{

e.preventDefault();

alert("Thank you for subscribing to Trey Mavrik's newsletter.");

});

}


/* Copyright */

console.log("Official Website of Trey Mavrik");


/* Current year */

const footer=document.querySelector("footer p");

if(footer){

footer.innerHTML="© "+new Date().getFullYear()+" Trey Mavrik. All Rights Reserved.";

}
