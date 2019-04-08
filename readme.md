# Voyager Page Modals

[![Latest Version on Packagist][ico-version]][link-packagist]
[![Total Downloads][ico-downloads]][link-downloads]
[![Build Status][ico-travis]][link-travis]
[![StyleCI][ico-styleci]][link-styleci]

This is where your description should go. Take a look at [contributing.md](contributing.md) to see a to do list.

## Prerequisites

- Composer Installed
- [Install Laravel](https://laravel.com/docs/installation)
- [Install Voyager](https://github.com/the-control-group/voyager)
- [Install Voyager Frontend](https://github.com/pvtl/voyager-frontend)
- [Install Voyager Page Blocks](https://github.com/pvtl/voyager-page-blocks)

## Installation

Via Composer

1. Require this package in your project
``` bash
composer require ctrlwebinc/voyager-page-modals
```
2. Add the following block to your project's config/page-blocks.php file
```php
$blocks['block-modal'] = [
    'name' => 'Modal',
    'template' => 'voyager-page-modals::block-modal',
    'fields' => [
        'saison' => [
            'field' => 'saison',
            'display_name' => 'Modal',
            'partial' => 'voyager-page-modals::formfields.modal-selector',
            'required' => 1,
        ],
    ],
];

```

## Usage

## Change log

Please see the [changelog](changelog.md) for more information on what has changed recently.

## Testing

``` bash
$ composer test
```

## Contributing

Please see [contributing.md](contributing.md) for details and a todolist.

## Security

If you discover any security related issues, please email info@ctrlweb.ca instead of using the issue tracker.

## Credits

- [ctrlweb][link-author]
- [All Contributors][link-contributors]

## License

MIT. Please see the [license file](license.md) for more information.

## Remerciements (yeah, we're French-speakers)

Merci au [Théâtre du Nouveau Monde][link-tnm], et à Olivier Chassé en particulier, pour son soutien dans le 
développement initial de ce projet. 

[ico-version]: https://img.shields.io/packagist/v/ctrlwebinc/voyager-page-modals.svg?style=flat-square
[ico-downloads]: https://img.shields.io/packagist/dt/ctrlwebinc/voyager-page-modals.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/ctrlwebinc/voyager-page-modals/master.svg?style=flat-square
[ico-styleci]: https://styleci.io/repos/179335461/shield

[link-packagist]: https://packagist.org/packages/ctrlwebinc/voyager-page-modals
[link-downloads]: https://packagist.org/packages/ctrlwebinc/voyager-page-modals
[link-travis]: https://travis-ci.org/ctrlwebinc/voyager-page-modals
[link-styleci]: https://styleci.io/repos/179335461
[link-author]: https://github.com/ctrlwebinc
[link-contributors]: ../../contributors
[link-tnm]: https://www.tnm.qc.ca
