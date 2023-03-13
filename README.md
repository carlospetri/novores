<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Checkout</title>
    <style>
        *{
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        .copy {
            font-size: 30px;
        }

        .like {
            width: 142px;
            height: 161px;
            object-fit: contain;
            margin-bottom: 30px;
        }
        .flex{
            text-align: center;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        .copy,.alt {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            font-size: 19.3px;
            font-weight: bold;
            font-style: normal;
            font-stretch: normal;
            line-height: normal;
            letter-spacing: 0.21px;
            text-align: center;
            color: #828282;
        }
        .alt {
            font-weight: normal;
        }

        #redirect{
            margin-top: 30px;
            display: inline-block;
            background-color: #5cb85d;
            text-decoration: none;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            font-size: 20px;
            font-weight: 500;
            font-style: normal;
            font-stretch: normal;
            line-height: 1.18;
            letter-spacing: 1.25px;
            text-align: center;
            color: #ffffff;
            padding: 15px 50px;
            border-radius: 20px;
            box-shadow: 0 5px 10px 2px rgba(0,0,0,0.3);
            transition: all 0.1s ease-in-out;
        }
        #redirect:hover{
            background-color: #3ea342;
            box-shadow: 0 5px 5px 2px rgba(0,0,0,0.3);
        }
    </style>
</head>
<body>
    <div class="flex">
        <div class="container">
            
            <p class="copy">
                Tudo certo!
            </p>
            <p class="alt">
                Clique em continuar para ser direcionado para a página solicitada.
            </p>
            <a href="#" id="redirect">Continuar</a>
        </div>
    </div>
    <script>
        var path = location.pathname+location.search;
        var monetizzepath  = 'https://app.monetizze.com.br/r/AFM22381020' + path;
        document.getElementById('redirect').setAttribute('href', monetizzepath);
    </script>
</body>
</html>
