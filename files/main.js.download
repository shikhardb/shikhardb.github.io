$(function() {
  "use strict";

  var window_width = $(window).width(),
    window_height = window.innerHeight,
    header_height = $(".default-header").height(),
    header_height_static = $(".site-header.static").outerHeight(),
    fitscreen = window_height - header_height,
    backtop = $("#back-top");

  /* ---------------------------------------------
        Wow js Start
     --------------------------------------------- */
  new WOW({
    mobile: false
  }).init();
  /* ---------------------------------------------
        Wow js End
     --------------------------------------------- */

  /* ---------------------------------------------
        Preloader Start
     --------------------------------------------- */
  $(window).on("load", function() {
    $(".se-pre-con").fadeOut("slow");
  });
  /* ---------------------------------------------
        Preloader End
     --------------------------------------------- */

  /* ---------------------------------------------
        scroll body to 0px on click Starts
     --------------------------------------------- */
  $("#back-top a").on("click", function() {
    $("body,html").animate(
      {
        scrollTop: 0
      },
      1000
    );
    return false;
  });
  /* ---------------------------------------------
  scroll body to 0px on click Ends
--------------------------------------------- */

  /* ---------------------------------------------
        Initiate superfish on nav menu Starts
     --------------------------------------------- */
  $(".nav-menu").superfish({
    animation: {
      opacity: "show"
    },
    speed: 400
  });
  /* ---------------------------------------------
        Initiate superfish on nav menu Ends
     --------------------------------------------- */

  /* ---------------------------------------------
        Navbar Active Class Start
     --------------------------------------------- */
  // Sciome 2
  $(".navbar-nav li a").on("click", function() {
    $("a").removeClass("active2");
    $(this).addClass("active2");
  });

  // Sciome 3 Menu active
  $(".side_menu .menu_right li").on("click", function() {
    $("li").removeClass("active3");
    $(this).addClass("active3");
  });

  // Sciome 4
  $(".nav4 a").on("click", function() {
    $(".nav4 a").removeClass("active4");
    $(this).addClass("active4");
  });

  // Sciome 5
  $(".navbar-nav .nav-item").on("click", function() {
    $(".nav-item").removeClass("active5");
    $(this).addClass("active5");
  });
  /* ---------------------------------------------
        Navbar Active Class End
     --------------------------------------------- */

  /* ---------------------------------------------
        Menubar Toggle
     --------------------------------------------- */
  // Sciome 2 Menubar
  $(".menu-bar2").on("click", function(e) {
    e.preventDefault();
    $(".navbar-nav").toggleClass("hide");
    $("span", this).toggleClass("lnr-menu lnr-cross");
  });

  // Sciome 4 Menubar
  $(".menu-bar4").on("click", function(e) {
    e.preventDefault();
    $(".nav4").toggleClass("hide");
    $("span", this).toggleClass("lnr-menu lnr-cross");
    $(".main-menu").addClass("mobile-menu");
  });
  /* ---------------------------------------------
        Menubar Toggle End
     --------------------------------------------- */

  /* ---------------------------------------------
        Banner Toggle Starts
     --------------------------------------------- */
  //  Open Socail Icons
  $(".open-social").on("click", function(e) {
    e.preventDefault();
    $(".social-profile").toggleClass("hide");
  });

  // Open Form Sciome 4
  $(".form-icon4").on("click", function(e) {
    e.preventDefault();
    $(".banner-form, .form-img").toggleClass("hide");
    $("span", this).toggleClass("lnr-envelope lnr-cross");
  });

  // Sciome 2 Banner
  $("#bannerForm").hide();
  $("#bannerContactClose").hide();
  $("#bannerContact").on("click", function() {
    $(this).fadeOut(400, function() {
      $("#bannerForm").fadeIn(700);
      $("#bannerContactClose").fadeIn(500);
    });
  });

  $("#bannerContactClose").on("click", function() {
    $(this).fadeOut(400, function() {
      $("#bannerContact").fadeIn(500);
      $("#bannerForm").fadeOut(700);
    });
  });

  // Sciome 2 About
  $("#aboutForm").hide();
  $("#aboutContactClose").hide();
  $("#aboutContact").on("click", function() {
    $(this).fadeOut(400, function() {
      $("#aboutForm").fadeIn(700);
      $("#aboutContactClose").fadeIn(500);
    });
  });

  $("#aboutContactClose").on("click", function() {
    $(this).fadeOut(400, function() {
      $("#aboutContact").fadeIn(500);
      $("#aboutForm").fadeOut(700);
    });
  });

  // Sciome 2 Resume
  $("#resumeForm").hide();
  $("#resumeContactClose").hide();
  $("#resumeContact").on("click", function() {
    $(this).fadeOut(400, function() {
      $("#resumeForm").fadeIn(700);
      $("#resumeContactClose").fadeIn(500);
    });
  });

  $("#resumeContactClose").on("click", function() {
    $(this).fadeOut(400, function() {
      $("#resumeContact").fadeIn(500);
      $("#resumeForm").fadeOut(700);
    });
  });

  // Sciome 2 Portfolio
  $("#portfolioForm").hide();
  $("#portfolioContactClose").hide();
  $("#portfolioContact").on("click", function() {
    $(this).fadeOut(400, function() {
      $("#portfolioForm").fadeIn(700);
      $("#portfolioContactClose").fadeIn(500);
    });
  });

  $("#portfolioContactClose").on("click", function() {
    $(this).fadeOut(400, function() {
      $("#portfolioContact").fadeIn(500);
      $("#portfolioForm").fadeOut(700);
    });
  });

  // Sciome 2 Contact
  $("#contactForm").hide();
  $("#contactContactClose").hide();
  $("#contactContact").on("click", function() {
    $(this).fadeOut(400, function() {
      $("#contactForm").fadeIn(700);
      $("#contactContactClose").fadeIn(500);
    });
  });

  $("#contactContactClose").on("click", function() {
    $(this).fadeOut(400, function() {
      $("#contactContact").fadeIn(500);
      $("#contactForm").fadeOut(700);
    });
  });
  /* ---------------------------------------------
        Banner Toggle Ends
     --------------------------------------------- */

  /* ---------------------------------------------
        Scrollyfy Starts
     --------------------------------------------- */
  // Sciome 1
  $(window)
    .on("scroll", function() {
      if ($(window).scrollTop() >= 100) {
        $("section").each(function(i) {
          if ($(this).position().top <= $(window).scrollTop() - 0) {
            $(".nav1 .nav-item.active1").removeClass("active1");
            $(".nav1 .nav-item")
              .eq(i)
              .addClass("active1");
          }
        });
      } else {
        $(".nav1 .nav-item.active1").removeClass("active1");
        $(".nav1 .nav-item:first").addClass("active1");
      }
    })
    .scroll();

  // Sciome 2
  $(window)
    .on("scroll", function() {
      if ($(window).scrollTop() >= 100) {
        $("section").each(function(i) {
          if ($(this).position().top > $(window).scrollTop()) {
            $(".nav-link2.active2").removeClass("active2");
            $(".nav-link2")
              .eq(i)
              .addClass("active2");
          }
        });
      } else {
        $(".nav-link2.active2").removeClass("active2");
        $(".nav-link2:first").addClass("active2");
      }
    })
    .scroll();

  // Sciome 3
  $(window)
    .on("scroll", function() {
      if ($(window).scrollTop() >= 100) {
        $("section").each(function(i) {
          if ($(this).position().top <= $(window).scrollTop() - 100) {
            $(".list3.active3").removeClass("active3");
            $(".list3")
              .eq(i)
              .addClass("active3");
          }
        });
      } else {
        $(".list3.active3").removeClass("active3");
        $(".list3:first").addClass("active3");
      }
    })
    .scroll();

  // Sciome 4
  $(window)
    .on("scroll", function() {
      if ($(window).scrollTop() >= 100) {
        $("section").each(function(i) {
          if ($(this).position().top <= $(window).scrollTop() - 0) {
            $(".nav4 a.active4").removeClass("active4");
            $(".nav4 a")
              .eq(i)
              .addClass("active4");
          }
        });
      } else {
        $(".nav4 a.active4").removeClass("active4");
        $(".nav4 a:first").addClass("active4");
      }
    })
    .scroll();

  // Sciome 5
  $(window)
    .on("scroll", function() {
      if ($(window).scrollTop() >= 100) {
        $("section").each(function(i) {
          if ($(this).position().top <= $(window).scrollTop() - 0) {
            $(".nav5 .nav-item.active5").removeClass("active5");
            $(".nav5 .nav-item")
              .eq(i)
              .addClass("active5");
          }
        });
      } else {
        $(".nav5 .nav-item.active5").removeClass("active5");
        $(".nav5 .nav-item:first").addClass("active5");
      }
    })
    .scroll();
  /* ---------------------------------------------
        Scrollyfy Ends
     --------------------------------------------- */

  /* ---------------------------------------------
       Smooth scroll for the menu Starts
    --------------------------------------------- */
  //  Sciome 1
  $(".nav1 .nav-item .nav-link").on("click", function(event) {
    if (this.hash !== "") {
      event.preventDefault();
      var hash = this.hash;
      $("html, body").animate(
        {
          scrollTop: $(hash).offset().top - -10
        },
        600,
        function() {
          window.location.hash = hash;
        }
      );
    }
  });

  $(".menu_nav .nav-item .nav-link, .nav-menu li a").on("click", function(
    event
  ) {
    if (this.hash !== "") {
      event.preventDefault();
      var hash = this.hash;
      $("html, body").animate(
        {
          scrollTop: $(hash).offset().top - -10
        },
        600,
        function() {
          window.location.hash = hash;
        }
      );
    }
  });

  $(".menu_right li a").on("click", function(event) {
    if (this.hash !== "") {
      event.preventDefault();
      var hash = this.hash;
      $("html, body").animate(
        {
          scrollTop: $(hash).offset().top - -10
        },
        800,
        function() {
          window.location.hash = hash;
        }
      );
    }
  });

  // Sciome 4
  $(".nav4 a").on("click", function(event) {
    if (this.hash !== "") {
      event.preventDefault();
      var hash = this.hash;
      $("html, body").animate(
        {
          scrollTop: $(hash).offset().top - -10
        },
        800,
        function() {
          window.location.hash = hash;
        }
      );
    }
  });
  /* ---------------------------------------------
       Smooth scroll for the menu Ends
    --------------------------------------------- */

  /* ---------------------------------------------
        Header Scroll
     --------------------------------------------- */
  // Sciome 1
  $(window).on("scroll", function() {
    if ($(this).scrollTop() > 100) {
      $("#header1").addClass("header-scrolled1");
      backtop.addClass("back-top-animation");
    } else {
      $("#header1").removeClass("header-scrolled1");
      backtop.removeClass("back-top-animation");
    }
  });

  // Sciome 3
  $(window).on("scroll", function() {
    if ($(this).scrollTop() - 0) {
      $(".header-top").addClass("header-scrolled4");
      backtop.addClass("back-top-animation");
    } else {
      $(".header-top").removeClass("header-scrolled4");
      backtop.removeClass("back-top-animation");
    }
  });

  // Sciome 5
  $(window).on("scroll", function() {
    if ($(this).scrollTop() > window_height - 60) {
      $("#header5").addClass("header-scrolled");
      backtop.addClass("back-top-animation");
    } else {
      $("#header5").removeClass("header-scrolled");
      backtop.removeClass("back-top-animation");
    }
  });
  /* ---------------------------------------------
        Header Scroll Ends
     --------------------------------------------- */

  /* ---------------------------------------------
        Owl Carousel
     --------------------------------------------- */
  $(".active-review-carusel").owlCarousel({
    items: 1,
    margin: 30,
    autoplay: true,
    loop: true,
    dots: true,
    stagePadding: 180,
    dots: true,
    responsive: {
      0: {
        items: 1,
        stagePadding: 0
      },
      1024: {
        items: 1,
        stagePadding: 180
      }
    }
  });

  $(".active-review-carusel5").owlCarousel({
    items: 1,
    margin: 30,
    autoplay: true,
    loop: true,
    dots: true,
    dots: true,
    animateOut: "slideOutUp",
    animateIn: "slideInUp"
  });

  $(".active-feedback-carusel").owlCarousel({
    loop: true,
    margin: 30,
    items: 2,
    nav: true,
    dots: false,
    responsiveClass: true,
    autoplay: 2500,
    slideSpeed: 300,
    paginationSpeed: 500,
    navText: [
      "<span class='lnr lnr-arrow-up'></span>",
      "<span class='lnr lnr-arrow-down'></span>"
    ],
    responsive: {
      0: {
        items: 1
      },
      1024: {
        items: 2
      }
    }
  });

  $(".active-project-carusel").owlCarousel({
    loop: true,
    margin: 30,
    items: 1,
    nav: false,
    dots: true,
    responsiveClass: true,
    autoplay: 2500,
    slideSpeed: 300,
    paginationSpeed: 500
  });

  $(".blog-banner-carusel").owlCarousel({
    loop: true,
    margin: 0,
    items: 1,
    nav: false,
    dots: true,
    responsiveClass: true,
    autoplay: 2500,
    slideSpeed: 300,
    paginationSpeed: 500,
    responsive: {
      0: {
        items: 1
      }
    }
  });

  $(".blog-post-carusel").owlCarousel({
    loop: true,
    margin: 0,
    items: 1,
    nav: false,
    dots: true,
    responsiveClass: true,
    autoplay: 2500,
    slideSpeed: 300,
    paginationSpeed: 500,
    responsive: {
      0: {
        items: 1
      }
    }
  });

  $(".slider_widget").owlCarousel({
    loop: true,
    margin: 0,
    items: 1,
    nav: false,
    dots: true,
    responsiveClass: true,
    autoplay: 2500,
    slideSpeed: 300,
    paginationSpeed: 500,
    responsive: {
      0: {
        items: 1
      }
    }
  });
  /* ---------------------------------------------
        Owl Carousel Ends
     --------------------------------------------- */

  /* ---------------------------------------------
        Progress Bar Starts
     --------------------------------------------- */
  // Version4
  var $progressBars = $(".progress-bars");
  $progressBars.find(".progress-bar").each(function() {
    var $t4 = $(this);
    $t4.css("width", 0);
    $t4.waypoint(
      function() {
        $t4.css("width", $t4.data("value") + "%");
      },
      {
        triggerOnce: true,
        offset: "bottom-in-view"
      }
    );
  });
  /* ---------------------------------------------
        Progress Bar Ends
     --------------------------------------------- */

  /* ---------------------------------------------
        Counter js Starts
     --------------------------------------------- */
  $(window).on("load", function() {
    $(".counter").counterUp({
      delay: 10,
      time: 1500
    });
  });
  /* ---------------------------------------------
        Counter js Ends
     --------------------------------------------- */

  /* ---------------------------------------------
            Isotope js Starts
         --------------------------------------------- */
  $(window).on("load", function() {
    $(".work-filter ul li").on("click", function() {
      $(".work-filter ul li").removeClass("active");
      $(this).addClass("active");

      var data = $(this).attr("data-filter");
      $workGrid.isotope({
        filter: data
      });
    });

    if (document.getElementById("portfolio")) {
      var $workGrid = $(".work-grid").isotope({
        itemSelector: ".all",
        percentPosition: true,
        masonry: {
          columnWidth: ".all"
        }
      });
    }
  });
  /* ---------------------------------------------
            Isotope js Ends
         --------------------------------------------- */

  /* ---------------------------------------------
            Fullpage js Starts
         --------------------------------------------- */
  //  Sciome 2
  if ($(window).width() < 1024) {
    $("#main2").removeAttr("id");
  }
  if (document.getElementById("main2")) {
    $("#main2").fullpage({
      sectionSelector: ".vertical-scrolling",
      navigation: false,
      slidesNavigation: true,
      controlArrows: false,
      keyboardScrolling: true,
      anchors: [
        "firstSection",
        "secondSection",
        "thirdSection",
        "fourthSection",
        "fifthSection"
      ],
      menu: "#menu"
    });
  }

  /* ---------------------------------------------
            Fullpage js Ends
         --------------------------------------------- */

  /* ---------------------------------------------
            Magnific Popup js Starts
         --------------------------------------------- */
  $(".img-gal").magnificPopup({
    type: "image",
    gallery: {
      enabled: true
    }
  });

  $(".play-btn").magnificPopup({
    type: "iframe",
    mainClass: "mfp-bg",
    removalDelay: 160,
    preloader: false,
    fixedContentPos: true
  });
  /* ---------------------------------------------
            Magnific Popup js Ends
         --------------------------------------------- */
});
