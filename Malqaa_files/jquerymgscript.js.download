$(document).ready(function () {

	// если отсутсвует zoomsl-3.0.min.js
	if (!$.fn.imagezoomsl) {

		$('.msg').show();
		return;
	}
	else $('.msg').hide();


	// инициализация плагина
	$('.my-foto').imagezoomsl({

		innerzoommagnifier: true,
		classmagnifier: window.external ? "round-loope" : "", // fix для Opera и Safary
		magnifierborder: "5px solid #F0F0F0",                 // fix для Opera и Safary		  
		zoomrange: [1],
		zoomstart: 2,
		magnifiersize: [200, 200]
	});  

 
});
