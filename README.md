# gRowing

As coisas ainda estão em desenvolvimento, por tanto documentarei tudo aqui

Todos os modulos podem ser usados tanto com JavaScript puro quanto com jQuery
Atualmente ha quatro modulos, ainda em expansão, são eles:
	Slides
	Modal
	Notify
	Form

Slides
	O modulo de slides por enquanto possui somente um modo, o banner,
	suas opções são:
			target:       //=> indica em qual div deve ser colocado os slides
			imagesUrl:    //=> caminho das imagens
			auto:         //=> se os slides devem passar automaticamente
			timeAuto:     //=> a cada quanto tempo os slides devem mudar
			autoExecute:  //=> indica se deve executar após estanciar a classe
			slideCount:   //=> diz se deve ter o contador de slides
			dots:         //=> indica se deve ter as bolinahs em baixo

	Se nenhuma url for passada, ele vai buscar nos filhos da div destino pelas imagens, e usar as que estão la

	Seu uso em JavaScript puro é mais ou menos assim:
		var mySlide = new SlideShow({
				//aqui se passa as opções
			});

	E em jQuery:
		$("#slide_show").slide_show({
			// Aqui vem as opções
		});
		onde #slide_show é o destino
		