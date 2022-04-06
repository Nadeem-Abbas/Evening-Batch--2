(function($){

	var yoast = {
		accordion: function(){
			$('.wp-block-yoast-faq-block').find('.schema-faq-question').click(function(){
				//Expand or collapse this panel
				$(this).nextAll('.schema-faq-answer').eq(0).slideToggle('fast', function(){
					if( $(this).hasClass('collapse') ){
						$(this).removeClass('collapse');
					}
					else{
						$(this).addClass('collapse');
					}
				});
			
				//Hide the other panels
				$(".schema-faq-answer").not( $(this).nextAll('.schema-faq-answer').eq(0) ).slideUp('fast');
			});

			$('.wp-block-yoast-faq-block .schema-faq-question').click(function(){
				$('.wp-block-yoast-faq-block .schema-faq-question').not( $(this) ).removeClass('collapse');
				if( $(this).hasClass('collapse') ){
					$(this).removeClass('collapse');
				}
				else{
					$(this).addClass('collapse');
				}
			});
		}
	};

	yoast.accordion();

})(jQuery)