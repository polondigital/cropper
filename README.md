# Cropper @Polon

[![Maintainer](http://img.shields.io/badge/maintainer-@polondigital-blue.svg?style=flat-square)](https://twitter.com/polondigital)
[![Source Code](http://img.shields.io/badge/source-polon/cropper-blue.svg?style=flat-square)](https://github.com/polondigital/cropper)
[![PHP from Packagist](https://img.shields.io/packagist/php-v/polon/cropper.svg?style=flat-square)](https://packagist.org/packages/polon/cropper)
[![Latest Version](https://img.shields.io/github/release/polondigital/cropper.svg?style=flat-square)](https://github.com/polondigital/cropper/releases)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE)
[![Build](https://img.shields.io/scrutinizer/build/g/polondigital/cropper.svg?style=flat-square)](https://scrutinizer-ci.com/g/polondigital/cropper)
[![Quality Score](https://img.shields.io/scrutinizer/g/polondigital/cropper.svg?style=flat-square)](https://scrutinizer-ci.com/g/polondigital/cropper)
[![Total Downloads](https://img.shields.io/packagist/dt/polon/cropper.svg?style=flat-square)](https://packagist.org/packages/polon/cropper)

###### Cropper is a component that simplifies the creation of JPG and PNG image thumbnails with a cache engine. Cropper CC creates your image for each part required in the application with zero complexity.

Cropper é um componente que simplifica a criação de miniaturas de imagens JPG e PNG com um motor de cache. O Cropper CC cria versões de suas imagens para cada dimensão necessária na aplicação com zero de complexidade.

####WEBP THUMBNAILS:

Published in version 1.3.* by default how thumbnails are converted to webP.

Adicionado na versão 1.3.* por padrão as miniaturas são convertidas para webP.

## About Polon

###### Polon is a set of small and optimized PHP components for common tasks. Held by Victor and the Polon team. With them you perform routine tasks with fewer lines, writing less and doing much more.

Polon é um conjunto de pequenos e otimizados componentes PHP para tarefas comuns. Mantido por Victor e a equipe Polon. Com eles você executa tarefas rotineiras com poucas linhas, escrevendo menos e fazendo muito mais.

### Highlights

- Simple Thumbnail Creator (Simples criador de miniaturas)
- Cache optimization per dimension (Otimização em cache por dimensão)
- Media Control by Filename (Contrôle de mídias por nome do arquivo)
- Cache cleanup by filename and total (Limpeza de cache por nome de arquivo e total)
- Composer ready and PSR-2 compliant (Pronto para o composer e compatível com PSR-2)

## Installation

Cropper is available via Composer:

```bash
"polon/cropper": "1.3.*"
```

or run

```bash
composer require polon/cropper
```

## Documentation

###### They are just two methods to do all the work. You just need to call ***make*** to create or use thumbnails of any size, or ***flush*** to free the cache of a file or the entire folder. Polon Cropper works like this:

São apenas dois métodos para fazer todo o trabalho. Você só precisa chamar o ***make*** para criar ou usar miniaturas de qualquer tamanho, ou o ***flush*** para liberar o cache de um arquivo ou da pasta toda. Polon Cropper funciona assim:

#### Create thumbnails

```php
<?php
require __DIR__ . "/../src/Cropper.php";

$c = new \Polon\Cropper\Cropper("patch/to/cache");

echo "<img src='{$c->make("images/image.jpg", 500)}' alt='Happy Coffee' title='Happy Coffee'>";
echo "<img src='{$c->make("images/image.jpg", 500, 300)}' alt='Happy Coffee' title='Happy Coffee'>";
```

#### Clear cache

```php
<?php
require __DIR__ . "/../src/Cropper.php";

$c = new \Polon\Cropper\Cropper("patch/to/cache");

//flush by filename
$c->flush("images/image.jpg");

//flush cache folder
$c->flush();
```

## Contributing

Please see [CONTRIBUTING](https://github.com/polondigital/cropper/blob/master/CONTRIBUTING.md) for details.

## Support

###### Security: If you discover any security related issues, please email polon@polon.digital instead of using the issue tracker.

Se você descobrir algum problema relacionado à segurança, envie um e-mail para polon@polon.digital em vez de usar o rastreador de problemas.

Thank you

## Credits

- [Victor](https://github.com/polondigital) (Developer)
- [Polon Treinamentos](https://github.com/polon) (Team)
- [All Contributors](https://github.com/polondigital/cropper/contributors) 

## License

The MIT License (MIT). Please see [License File](https://github.com/polondigital/cropper/blob/master/LICENSE) for more information.