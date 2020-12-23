$(document).ready(function()
{
	var containers = $(".owlllheight");
    for (var i = containers.length - 1; i >= 0; i--) 
 {
	var cw, ch, iw, ih, nw, nh;  //container (c), image (i), and new (n) height (h) and width (w)
		var img = $(containers[i]).find("img");
		cw = $(containers[i]).width();
		ch = $(containers[i]).height();
	containers.css("overflow","hidden");

	if(img.length==1)
	{
	 
		iw = $(img).width();
		ih = $(img).height();
	 
		$(img).css("position","relative");

	 if(iw/ih > cw/ch) //in this case the height of the image will be same as container and width will overflow
	 {
	 	//nh=ch;
	 	//nw=(iw/ih)*nh;
	 	//var left = -(nw-cw)/2;
		 //$(img).css("left",left+"px");
	 }
	 else
	 {
	 	nw=cw;
	 	nh=(ih/iw)*nw;
	 	var top= -(nh-ch)/2;
		 $(img).css("top",top+"px");
	 }

		$(img).width(nw);
		$(img).height(nh);

	}

 }

});