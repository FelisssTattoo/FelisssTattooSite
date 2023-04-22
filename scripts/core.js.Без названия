var src = "https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2605.711407059518!2d28.42310861568737!3d49.22499997932504!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x472d5d29238d478f%3A0xc281340939da3b77!2sTATTOO%20LAMARCH%20STUDIO!5e0!3m2!1sru!2sua!4v1570812057149!5m2!1sru!2sua";

$(document).ready(function() {
	$(".map > iframe").attr("src", src);
});

[].forEach.call(document.querySelectorAll('img[data-src]'), function(img) {
	img.setAttribute('src', img.getAttribute('data-src'));
		img.onload = function() {
		img.removeAttribute('data-src');
	};
});
$(document).ready(function() {
	function imRes(){
		let $w = $('.sec5-gallery-img').width();
		$('.sec5-gallery-img').height($w);
	};
	imRes();
	$( window ).resize(function() {
		imRes();
	});
});

$('.sec3-items-wrap').slick({
	arrows: false,
	slidesToShow: 1,
	autoplay: true
});

// $('.nav-ul-li-a').on('click', function(e){
// 	let $ank = $(this).attr('hre');
// 	alert($ank);
// 	$('html,body').stop().animate({ scrollTop: $('#'.$ank.'').offset().top }, 1000);
// });

var $page = $('html, body');
$('a[href*="#"]').click(function() {
    $page.animate({
        scrollTop: $($.attr(this, 'href')).offset().top
    }, 400);
    return false;
});

$('.count').each(function () {
    $(this).prop('Counter',0).animate({
        Counter: $(this).text()
    }, {
        duration: 5000,
        easing: 'swing',
        step: function (now) {
            $(this).text(Math.ceil(now));
        }
    });
});

$('.h-burger').click(function(){
	$('.nav-ul.header').slideDown().css({"display":"flex"});
})

$('.nav-ul-li-a').click(function(){
	$('.nav-ul.header').slideDown().css({"display":"none"});
})

$('.nav-ul.header.exit').click(function(){
	$('.nav-ul.header').slideUp();
})