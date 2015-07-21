# webcomponent-minicart-example
Пример использования web components.

Этот пример я создал для того, чтобы показать, как просто и элегантно можно использовать web компоненты.

Для использования этого примера достаточно подключить к вашему проект мой html файл:

    <link rel="import" href="components/mini-cart.html"/>

И написать такой html код (ссылки тут просто для примера):

    <mini-cart cart-url="/cart" checkout-url="/checkout">
		<cart-item url="/product1" remove-url="/cart/?remove=product1">
			<product-image>http://enterprise-demo.user.magentotrial.com/media/catalog/product/cache/1/small_image/210x/9df78eab33525d08d6e5fb8d27136e95/m/s/msj012t_2.jpg</product-image>
			<name>Product Example</name>
			<qty>1</qty>
			<price>$120</price>
		</cart-item>
		<cart-item url="/product2" remove-url="/cart/?remove=product2">
			<product-image>http://enterprise-demo.user.magentotrial.com/media/catalog/product/cache/1/small_image/210x/9df78eab33525d08d6e5fb8d27136e95/m/t/mtk004t.jpg</product-image>
			<name>Product Example 2</name>
			<qty>2</qty>
			<price>$250</price>
		</cart-item>
		<total>$500</total>
    </mini-cart>
  
  На данный момент, из коробки, пример работать будет только в Google Chrome, но для остальных браузеров можно подключить специальные полифилы:
  
    <script src="https://cdnjs.cloudflare.com/ajax/libs/webcomponentsjs/0.7.7/webcomponents.min.js"></script>

Список поддерживаемых браузеров можно посмотреть тут:
https://github.com/webcomponents/webcomponentsjs/#browser-support
