# Vendors

Most projects will have a `vendors/` folder containing all the CSS files from external libraries and frameworks – Normalize, Bootstrap, jQueryUI, FancyCarouselSliderjQueryPowered, and so on. Putting those aside in the same folder is a good way to say “Hey, this is not from me, not my code, not my responsibility”.

If you have to override a section of any vendor, I recommend you have an 8th folder called `vendors-extensions/` in which you may have files named exactly after the vendors they overwrite. For instance, `vendors-extensions/_bootstrap.scss` is a file containing all CSS rules intended to re-declare some of Bootstrap’s default CSS. This is to avoid editing the vendor files themselves, which is generally not a good idea.

И последнее, но не менее важное, большинство проектов будут иметь папку vendors/, содержащую все CSS-файлы из внешних библиотек и фреймворков – Normalize, Bootstrap, jQueryUI, FancyCarouselSliderjQueryPowered и так далее. Нахождение этих файлов в этой папке – хороший способ сказать: “Эй, это не я писал, не мой код, не моя ответственность”.

    _normalize.scss
    _bootstrap.scss
    _jquery-ui.scss
    _select2.scss

Если вы хотите что-то переопределить в файлах любого вендора, то я рекомендую вам ввести восьмую папку vendors-extensions/, в которой вы будете хранить файлы с точно такими же именами, что и файлы, которые они переопределяют.

Например, файл vendors-extensions/_boostrap.scss, содержит все CSS-правила, переопределящие стандартные CSS-правила Bootstrap. Это сделано для того, чтобы не править сами внешние модули, что является совсем не здоровской идеей.