$(document).ready(function(){
	$( ".header-bottom-right-menu ul li:last-child" ).click(function() {
	  $("ul.sub-menu" ).slideToggle();
	});
	
	function createOptions(number) {
	var options = [], _options;

	  for (var i = 0; i < number; i++) {
		var option = '<option value="' + i + '">Option ' + i + '</option>';
		options.push(option);
	  }

	  _options = options.join('');
	  $('#number2')[0].innerHTML = _options;
	   $('.selectstyle')[0].innerHTML = _options;
	  
	}
	
		$('input[type=radio]').change(function()
	{
		if (this.checked)
		{
			$(this).closest('.form-group')
				.find('input[type=radio]').not(this)
				.prop('checked', false);
		}
	});


	$('.view-selection a').on('click',function(e) {
    if ($(this).hasClass('grid')) {
        $('.products>ul').removeClass('list').addClass('grid');
		$('.col-md-8').removeClass('padding-left-zero');
    }
    else if($(this).hasClass('list')) {
        $('.products>ul').removeClass('grid').addClass('list');
		$('.col-md-8').addClass('padding-left-zero');
    }
	});
});


$(document).ready(function () {
	$('.toast__close').click(function (e) {
		e.preventDefault();
		var parent = $(this).parent('.toast');
		parent.fadeOut("slow", function () { $(this).remove(); });
	});

	$('.searchedoption__radio__btn').click(function () {
		if ($('.searchedoption__radio__btn').is(':checked')) {
			$("#addcreationpop__form .form-group").removeClass("greenborder");
			//var value = $(this).val();
			//alert(value);
			$(this).parent().addClass("greenborder");
			
		}
	});

	//$("button.save__this__search__btn").click(function () {
	//	$("#_").text(function (i, j) {
	//		return j === '+' ? '-' : '+'
	//	});
	//	$("button.save__this__search__btn span.btn_text").text(function (i, v) {
	//		return v === 'Save this search' ? 'Remove this search' : 'Save this search'
	//	});
	//});

	
});



