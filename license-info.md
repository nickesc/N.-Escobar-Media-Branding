# License documentation for N. Escobar Media

## Setup
To get license templates, navigate to the project directory and use:
``` cmd
git clone https://github.com/nickesc/license-templates
```

Licenses can be generated using `lice`
To install `lice` use `pip`
``` cmd
pip install lice
```


When `lice` is installed, you can use these commands to generate licenses:


## Usage

```cmd
lice -o [AUTHOR] -p [PROJECT_NAME] -t license-templates/[LICENSE_NAME].txt -f [FILE_NAME]
```

## License Options:

### 1. `apache`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/apache.txt -f LICENSE
```

> A permissive license whose main conditions require preservation of copyright and license notices. Contributors provide an express grant of patent rights. Licensed works, modifications, and larger works may be distributed under different terms and without source code.

### 2. `bsd3`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/bsd3.txt -f LICENSE
```

> This license allows you almost unlimited freedom with the software so long as you include the BSD copyright and license notice in it, and do not use the author's name to endorse or promote your work without written permission.

### 3. `cc0`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/cc0.txt -f LICENSE
```

> No copyright, dedicates the work to public domain. You can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission.

### 4. `cc0_software`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/cc0_software.txt -f LICENSE
```

> The software version of `cc0`, dedicates the software to the public domain. Not approved by OSI. The `[ description ]` and `[ organizationEmail ]` fields must be filled in.

### 5. `cc_by`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/cc_by.txt -f LICENSE
```

> This license lets others distribute, remix, adapt, and build upon your work, even commercially, as long as they credit you for the original creation. This is the most accommodating of licenses offered. Recommended for maximum dissemination and use of licensed materials.

### 6. `cc_by_nc`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/cc_by_nc.txt -f LICENSE
```

> This license lets others remix, adapt, and build upon your work non-commercially, and although their new works must also acknowledge you and be non-commercial, they don’t have to license their derivative works on the same terms.

### 7. `cc_by_nc_nd`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/cc_by_nc_nd.txt -f LICENSE
```

> This license is the most restrictive of our six main licenses, only allowing others to download your works and share them with others as long as they credit you, but they can’t change them in any way or use them commercially.

### 8. `cc_by_nc_sa`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/cc_by_nc_sa.txt -f LICENSE
```

> This license lets others remix, adapt, and build upon your work non-commercially, as long as they credit you and license their new creations under the identical terms.

### 9. `cc_by_nd`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/cc_by_nd.txt -f LICENSE
```

> This license lets others reuse the work for any purpose, including commercially; however, it cannot be shared with others in adapted form, and credit must be provided to you.

### 10. `cc_by_sa`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/cc_by_sa.txt -f LICENSE
```

> This license lets others remix, adapt, and build upon your work even for commercial purposes, as long as they credit you and license their new creations under the identical terms. This license is often compared to “copyleft” free and open source software licenses. All new works based on yours will carry the same license, so any derivatives will also allow commercial use. This is the license used by Wikipedia, and is recommended for materials that would benefit from incorporating content from Wikipedia and similarly licensed projects.

### 11. `gpl3`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/gpl3.txt -f LICENSE
```

> Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights.

### 12. `mit`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/mit.txt -f LICENSE
```

> A short and simple permissive license with conditions only requiring preservation of copyright and license notices. Licensed works, modifications, and larger works may be distributed under different terms and without source code.

### 13. `unlicense`

```cmd
lice -o "N. Escobar Media" -p [PROJECT_NAME] -t license-templates/unlicense.txt -f LICENSE
```

> A license with no conditions whatsoever which dedicates works to the public domain. Unlicensed works, modifications, and larger works may be distributed under different terms and without source code.


## Reference
### `lice` Usage
> ```
> usage: lice [-h] [-o ORGANIZATION] [-p PROJECT] [-t TEMPLATE_PATH] [-y YEAR]
>             [--vars] [license]
> 
> positional arguments:
>   license               the license to generate, one of: agpl3, apache, bsd2,
>                         bsd3, cddl, cc0, epl, gpl2, gpl3, lgpl, mit, mpl
> 
> optional arguments:
>   -h, --help            show this help message and exit
>   -o ORGANIZATION, --org ORGANIZATION
>                         organization, defaults to .gitconfig or
>                         os.environ["USER"]
>   -p PROJECT, --proj PROJECT
>                         name of project, defaults to name of current directory
>   -t TEMPLATE_PATH, --template TEMPLATE_PATH
>                         path to license template file
>   -y YEAR, --year YEAR  copyright year
>   -l LANGUAGE, --language LANGUAGE
>                         format output for language source file, one of: js, f,
>                         css, c, m, java, py, cc, h, html, lua, erl, rb, sh,
>                         f90, hpp, cpp, pl, txt [default is not formatted (txt)]
>   -f OFILE, --file OFILE Name of the output source file (with -l, extension can be omitted)
>   --vars                list template variables for specified license
> ```