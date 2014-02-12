Redux extension-loader
================

The loader code needed to instantiate any Redux extension. To load any Redux extension, you need but do two things:

* Inside loader.php change `{$redux_opt_name}` to match your opt_name or set `$redux_opt_name` to your `opt_name` and make sure it's accessible by loader.php.
* Change the function name and hook reference of `redux_register_custom_extension_loader` as not to conflict with another developer's code.

Then place any extension folder within ~/extensions.

Depending on the extension you may also need to load a config file of some type to declare the options for that extension.