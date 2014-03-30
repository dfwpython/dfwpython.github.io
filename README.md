DFWPythoneers Website
=====================

This is the website for DFWPythoneers using Pelican.

GitHub Pages
------------

The master branch is the compiled output from Pelican for hosting through GitHub Pages.
Due to this, the development branch containing the Peclican files is renamed to pelican-master.
Care must be taken when working with the repository.


Usage
-----
```bash
git clone https://github.com/dfwpython/dfwpython.github.io.git
cd dfwpython.github.io
git checkout pelican-master <- the pelican project
virtualenv ./
pip install -r requirements.dev.txt
cd dfwpython-web

…update site content…

make publish
git status/git commit -a
cd ..
git checkout master <— master has the generated content
cp -R dfwpython-web/output/* ./
git status/git commit -a
git push origin master <- publishes content
git push origin pelican-master
```

Other Notes
-----------

The template is based off of the [zurb-F5-basic theme](https://github.com/getpelican/pelican-themes/tree/master/zurb-F5-basic)
The files were updated with the latest distribution of [Zurb Foundation 5](http://foundation.zurb.com/)


License
-------

Unless otherwise stated. The content of this repository is Copyright 2014 DFWPythoneers and its contributors.
A license to use the source code is issued under a BSD-3-Clause license. Further, any content that does not constitute
source code and not covered under a specified licenese, is licensed under a Creative Commons Attribution Share-Alike 3.0
[CC BY-NC-SA 3.0 US](https://creativecommons.org/licenses/by-nc-sa/3.0/us/).


BSD 3-Clause License

Copyright (c) 2014, DFWPythoneers and contributors
All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.