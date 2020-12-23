
        $('#select_language').on('change', function () {
            $("body").removeClass();
            var languageclass = this.value;
            $("body").addClass(languageclass);
            if ($("body").hasClass("arabic")) {
                $(".right-side-section-area").addClass("arabic-v");
                $(".header-right-menu").removeClass("text-right");
                $(".header-bottom-right-menu").removeClass("text-right");
                
            } else if ($("body").hasClass("English")) {
                $(".right-side-section-area").removeClass("arabic-v");
                $(".header-right-menu").addClass("text-right");
                $(".header-bottom-right-menu").addClass("text-right");
            }
        });
