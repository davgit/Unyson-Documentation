Theme
=====

The theme's manifest is located in ``framework-customizations/theme/manifest.php`` and can be accessed like this:

.. code-block:: php

    fw()->theme->manifest->get('version');

It supports the following parameters:

.. code-block:: php

    <?php if (!defined('FW')) die('Forbidden');

    $manifest = array();

    $manifest['id']           = 'theme-id';
    $manifest['name']         = __('Theme Title', 'fw');
    $manifest['uri']          = 'http://themefuse.com/wp-themes-shop/theme-name';
    $manifest['description']  = __('Another awesome wordpress theme', 'fw');
    $manifest['version']      = '1.0';
    $manifest['author']       = 'ThemeFuse';
    $manifest['author_uri']   = 'http://themefuse.com/';
    $manifest['requirements'] = array(
        'wordpress' => array(
            'min_version' => '3.9',
            /*'max_version' => '1000.0.0'*/
        ),
        'framework' => array(
            /*'min_version' => '0.0.0',
            'max_version' => '1000.0.0'*/
        ),
        'extensions' => array(
            /*'extension_name' => array(
                'min_version' => '0.0.0',
                'max_version' => '1000.0.0'
            )*/
        )
    );