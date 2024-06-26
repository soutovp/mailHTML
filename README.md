## Mail Marketing

Estrutura BASE para desenvolver um HTML para e-mail marketing

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
	<head>
		<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
		<meta http-equiv="X-UA-Compatible" content="IE=edge" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>SailChimp HTML Email Template</title>
		<style type="text/css">
			@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@700&display=swap');
			body {
				margin: 0;
			}
			table {
				border-spacing: 0;
			}
			td {
				padding: 0;
			}
			img {
				border: 0;
			}
		</style>
	</head>
	<body>
		<center class="wrapper">
			<table class="main" width="100%">
				<!-- BORDER -->

				<!-- LOGO & SOCIAL MEDIA SECTION -->

				<!-- BANNER IMAGE -->

				<!-- TITLE, TEXT & BUTTON -->

				<!-- BORDER -->

				<!-- THREE COLUMN SECTION -->

				<!-- BORDER -->

				<!-- TWO COLUMN SECTION -->

				<!-- FOOTER SECTION -->
			</table>
			<!-- End Main Class -->
		</center>
		<!-- End Wrapper -->
	</body>
</html>
```

## Criando um container principal

```html
<style>
	.wrapper {
		width: 100%;
		table-layout: fixed;
		background-color: cor-desejada;
		padding-bottom: 60px; /*Adiciona um espaçamento no final*/
	}
</style>
```

```html
<center class="wrapper"></center>
```

## Criando um container para centralizar as informações para corpo de E-mail

```css
.main {
	width: 100%;
	max-width: 600px;
	background-color: #fff;
	font-family: sans-serif;
	color: #4a4a4a;
	box-shadow: 0 0 25px rgba(0, 0, 0, 0.15);
	text-align: center;
}
```

```html
<table class="main" width="100%">
	<tr>
		<td></td>
	</tr>
</table>
```

Agora para cada elemento dentro do corpo do nosso e-mail, terá um TR (table row) e TD ( table data ).

## Criando borda ou linha para a tabela

```html
<tr>
	<td height="8" style="background-color: #000"></td>
</tr>
```

Percebe que estilização do próprio container TD, é feito dentro da tag TD.

## Alinhando elementos dentro de um container!

Primeiro vamos criar nossa sessão :

```html
<tr>
	<td style="padding: 14px 0 4px"></td>
</tr>
```

Nesta sessão, vimos que tem um padding para o distanciamento dos elementos internos das bordas.

A partir de agora, vamos criar um novo container interno para definir que nossa sessão terão duas colunas:

```css
.two-columns {
	font-size: 0;
	text-align: center;
}
```

```html
<tr>
	<td style="padding: 14px 0 4px">
		<table style="width: 100%">
			<tr>
				<td ckass="two-columns"></td>
			</tr>
		</table>
	</td>
</tr>
```
