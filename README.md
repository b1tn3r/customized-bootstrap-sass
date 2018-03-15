# Custom Bootstrap Sass Template

Custom setup for adding bootstrap's sass styles to a project and allows for easy disabling of parts of bootstrap that are not used in a project. Also contains built-in bootswatch configuration that already has the template to configured to the "Slate" theme, in which only the theme name needs to be exchanged for a different one. 

All the content is already displayed or commented out including any bootstrap variables, mixins, utilities or bootswatch themes.

## Usage

- Add this to a project that is using bootstrap and/or a bootswatch theme and make 'styles.scss' the entry file for compiling to CSS, which will link to both bootstrap and bootswatch.

- Tried and tested in React/Redux, but will also work in many other environments especially if they are connected to webpack. Be sure to add 'styles.scss' to the dependency tree and all the sass will compile with both bootstrap and bootswatch.

- '_bootstrap.scss' is the controller for all the bootstrap imports, while 'styles.scss' controls bootstrap, bootswatch, and all other project-specific imports. Be sure to comment out any components/utilities in _bootstrap.scss that are not being used by your project, as this will save several KB of space in the resulting compiled CSS file.

- If you want a theme other than "slate" then go into 'styles.scss' and change the imports '~bootswatch/dist/slate/variables' and '~bootswatch/dist/slate/bootswatch' to '~bootswatch/dist/[theme_name]/variables' and '~bootswatch/dist/[theme_name]/bootswatch'.

- If you want to change other bootstrap built-in variables, you can make these changes in '_variables.scss' where you can see all the default bootstrap values commented out. Uncomment these values and change them to your desired styles. 


## Authors

* **Mike** - *Founder of Titan Global Tech* - [b1tn3r](https://github.com/b1tn3r)
* **Titan Global Tech** - [titanglobaltech.net](http://titanglobaltech.net)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details