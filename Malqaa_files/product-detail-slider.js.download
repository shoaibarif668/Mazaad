
var sync12 = $("#detailslidermain");
var sync22 = $("#detailsliderthumb");

var thumbnailItemClass = '.owl-item';

var slides;

function detailslider(rtltype) {

     slides = sync12.owlCarousel({
     video: true,
         lazyLoad: true,
         onTranslated: function () {
             // Update Magnify when slide changes
             $zoom.destroy().magnify();
         },
        
     items: 1,
     margin: 10,
     nav: true,
     rtl: rtltype,
     transitionStyle: "fade",
     dots: false
     }).on('changed.owl.carousel', syncPosition);
   

}



function syncPosition(el) {
    $owl_slider = $(this).data('owl.carousel');
    var loop = $owl_slider.options.loop;

    if (loop) {
        var count = el.item.count - 1;
        var current = Math.round(el.item.index - (el.item.count / 2) - .5);
        if (current < 0) {
            current = count;
        }
        if (current > count) {
            current = 0;
        }
    } else {
        var current = el.item.index;
    }

    var owl_thumbnail = sync22.data('owl.carousel');
    var itemClass = "." + owl_thumbnail.options.itemClass;


    var thumbnailCurrentItem = sync22
        .find(itemClass)
        .removeClass("synced")
        .eq(current);

    thumbnailCurrentItem.addClass('synced');

    if (!thumbnailCurrentItem.hasClass('active')) {
        var duration = 300;
        sync22.trigger('to.owl.carousel', [current, duration, true]);
    }
}
var thumbs = sync22.owlCarousel({
    items: 5,
    lazyLoad: true,
    loop: false,
    transitionStyle: "fade",
    margin: 0,
    autoplay: false,
    nav: false,
    dots: false,
    onInitialized: function (e) {
        var thumbnailCurrentItem = $(e.target).find(thumbnailItemClass).eq(this._current);
        thumbnailCurrentItem.addClass('synced');
    },
}).on('click', thumbnailItemClass, function (e) {
        e.preventDefault();
        var duration = 300;
        var itemIndex = $(e.target).parents(thumbnailItemClass).index();
        sync12.trigger('to.owl.carousel', [itemIndex, duration, true]);
    }).on("changed.owl.carousel", function (el) {
        var number = el.item.index;
        $owl_slider = sync12.data('owl.carousel');
        $owl_slider.to(number, 100, true);
    });


$(".show___more button").click(function () {
    $(".show___more span i").toggleClass("rotate");
    $(".product____description___wrapper").toggleClass("fullheight");
    $(this).text($(this).text() == 'Show More' ? 'Show Less' : 'Show More');
});



$(".product-detail-info-wrapper").find('.print-link').on('click', function () {
    //Print ele2 with default options
    $.print(".product-detail-info-wrapper");
    
});

var maxLength = 500;
$('#comment__form textarea').keyup(function () {
    var textlen = maxLength - $(this).val().length;
    $('#rchars').text(textlen);
});

var url = $(location).attr('href');

$(".add__favourite___seller__btn button").click(function () {

        $(".add__favourite___seller__btn button span.btn__text").text(function (i, v) {
            return v === 'Add to Favourite Sellers' ? 'Remove from Favourite Sellers' : 'Add to Favourite Sellers'
        });
        $("#_ tspan").text(function (i, j) {
            return j === '+' ? '-' : '+'
        });

});

$("input#postquest").click(function () {
    $("#comment__form .form-group").removeClass("display-none")
});

$("input#postquestNew").click(function () {
    $("#comment__formNew .form-group").removeClass("display-none")
});



$(document).ready(function () {
    $(".tracker").click(function () {
        $('.owl-item.active a').trigger('click');
    });
});








