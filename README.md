# plaintext-everything

![version-control-everything](http://i.imgur.com/P0aDBIT.jpg)

A curated list of awesome plain-text tools.

I like to keep everything under version control as plain-text. This is a list of utilities that allow you to do that. Unmaintained tools are ~~striked out~~.

**Note**: \* denotes that the linked item is not a library or tool, but an article or blog post.

## DNS

 - [clouddns](https://github.com/jhawthorn/clouddns) (Cloudfront)
 - [namesync](https://github.com/dnerdy/namesync) (Cloudflare)
 - [Terraform](https://www.terraform.io/docs/providers/) has providers for CloudFlare, UltraDNS, and PowerDNS

## Configuration

- [etckeeper](https://etckeeper.branchable.com/). The [Arch Wiki](https://wiki.archlinux.org/title/Etckeeper) has a nice guide on usage.
- [NixOS](https://nixos.org/) is a completely declarative OS that uses `nix`, the purely functional package manager
- [RANCID](https://shrubbery.net/rancid/) -  RANCID monitors a device's configuration, including software and hardware (cards, serial numbers, etc) and uses a version-control-system to maintain history of changes.
- [Oxidised](https://github.com/ytti/oxidized) - Oxidized is a network device configuration backup tool. It's a RANCID replacement!
- \*[Blog post about Oxidised](https://log.cyconet.org/2016/01/29/oxidized-silly-attempt-at-really-awesome-new-cisco-config-differ/)
- In general, most [configuration management software](https://en.wikipedia.org/wiki/Comparison_of_open-source_configuration_management_software) will keep everything in plain-text.

## Terraform

Terraform lets you manage a lot of things in plain-text, including Cloud Assets, Databases, Networking, configuration for various Web services, your CI/CD configuration, and even your Google Calendar. A full list of providers is [on the Terraform Registry](https://registry.terraform.io/browse/providers).

## Passwords

- \*[Question](http://stackoverflow.com/questions/559611/password-storage-in-source-control) on StackOverflow
- \*John Resig's [blog post](http://ejohn.org/blog/keeping-passwords-in-source-control/)
- [pass](http://www.passwordstore.org/) - Standard unix password manager (encrypt, then commit).
- [ansible-vault](https://docs.ansible.com/playbooks_vault.html) - Encrypted storage for ansible.
- [sops](https://github.com/mozilla/sops) - Encrypts files for git.
## Dotfiles

- \*[dotfiles.github.io](https://dotfiles.github.io/) - List of various dotfile resources, curated by github
- \*[Arch Wiki Guide](https://wiki.archlinux.org/index.php/Dotfiles#Version_control) on using version control for dotfiles
- [gnu stow](http://www.gnu.org/software/stow/)

## Editors

- \*[http://www.terminally-incoherent.com/blog/2012/03/12/putting-your-vim-files-under-version-control/](putting-your-vim-files-under-version-control)
- [Editorconfig](http://editorconfig.org/) - Keep your coding styles in a .editorconfig file.

## Media

- [Git Large File Storage](https://git-lfs.github.com/) - Replaces large fileswith text pointers inside Git, while storing the file contents on a remote server. Maintained by github

## Encrypted Storage

- \*[HN Thread](https://news.ycombinator.com/item?id=8264496) for blackbox, with various alternatives suggested
- [git-crypt](https://www.agwa.name/projects/git-crypt/) - git-crypt enables transparent encryption and decryption of files in a git repository
- \*[Blog post](http://dsernst.com/2015/06/09/git-crypt-is-git--encryption/) on git-crypt
- [transcrypt](https://github.com/elasticdog/transcrypt) - transparently encrypt files within a git repository
- [blackbox](https://github.com/StackExchange/blackbox) - use decryption keys per user, meaning that there is no single shared password

## Designers

- [pixelapse](https://www.pixelapse.com/) - Visual version control and collaboration workflow
- \*[Adobe Version Cue](http://sixrevisions.com/project-management/the-ultimate-guide-to-version-control-for-designers/) - Blog post explaining version control to designers
- [kactus.io](https://kactus.io/) - Version control for designers (Sketch+Git for now)
- [SnowFS](https://github.com/Snowtrack/SnowFS) - a fast, scalable version control file storage for graphic files. There is a [commercial offering](https://www.snowtrack.io/) as well.

## Music

- [lilypond](http://www.lilypond.org/features.html) - version control for sheet music. Think Latex for sheet music
- [tunemachine](https://github.com/jez/tunemachine) - Version control for spotify playlists.

## Database

- \*Jeff Atwood's [blog post](http://blog.codinghorror.com/get-your-database-under-version-control/)
- [GNU Recutils](https://www.gnu.org/software/recutils/) - set of tools and libraries to access human-editable, plain text databases called recfiles. The data is stored as a sequence of records, each record containing an arbitrary number of named fields.

### Database Schema

- [flyway](https://flywaydb.org/) - Version control for your database.
- [MyBatis](http://www.mybatis.org/migrations/)
- [Liquibase](https://www.liquibase.org/) - Source Control for your database
- [Rumba RDBM](https://www.dbinvent.com/) - Database schema migration tool, plain-SQL, and declarative schema definition supported.

## Backups

- [bup](https://github.com/bup/bup) - Very efficient backup system based on the git packfile format, providing fast incremental saves and global deduplication (among and within files, including virtual machine images)

## Writing

- [Draft](https://draftin.com/) - Easy version control and collaboration for writers.
- [Penflip](https://www.penflip.com/) - GitHub for *collaborative* writers.
- [GitBook](https://www.gitbook.com/) - Book publishing platform based on git and markdown.
- [CriticMarkup](http://criticmarkup.com/) - a way for authors and editors to track changes to documents in plain text.

### Journaling
- [Journal.TXT](https://journaltxt.github.io/) - Single-Text File Journals.
- [journal-cli](https://journalcli.me/) - Index Your Markdown-Based Journal With Yaml Front Matter!

## Todo

- [todo.txt](http://todotxt.com/) - Pretty well known text file format with applications on many platforms.
- \*[Todo list in version control](http://urasaru.org/post/19414431348/getting-my-todo-list-under-version-control) - Based on using notational velocity and tracking it in git.

## Food

- ~~[Fork the Cookbook](http://forkthecookbook.com/) - GitHub for recipes~~
- ~~[diy.soylent](https://diy.soylent.com/) - Soylent recipes can be tracked and include changelogs. They can also be forked.~~
- [CookLang](https://cooklang.org/) - Recipe Markup Language

## Diagrams & Flowcharts

- [Web Sequence Diagrams](https://www.websequencediagrams.com/) - Generates imagess from your plain text descriptions. Has [an API](http://www.websequencediagrams.com/embedding.html) for plugin support, so you can embed easily.
- [Kanga Modelling](https://kangamodeling.codeplex.com/) - UML diagram generator in plain text. Written in .NET
- [yuml.me](http://yuml.me/) - Class UML diagrams, described in plain text, and easily embeddable.
- [Mermaid](https://mermaid-js.github.io/mermaid/#/) - Mermaid lets you create diagrams and visualizations using text and code.
- [Kroki](https://kroki.io/) - Kroki provides a unified API for all the diagram libraries including BlockDiag (BlockDiag, SeqDiag, ActDiag, NwDiag, PacketDiag, RackDiag), BPMN, Bytefield, C4 (with PlantUML), Ditaa, Erd, Excalidraw, GraphViz, Mermaid, Nomnoml, Pikchr, PlantUML, SvgBob, UMLet, Vega, Vega-Lite, WaveDrom... and more.
- [ditaa](http://ditaa.sourceforge.net/) - converts diagrams drawn using ascii art, into proper bitmap graphics.
- [erd](https://github.com/BurntSushi/erd) - takes a plain text description of entities, their attributes and the relationships between entities and produces a visual diagram modeling the description using GraphViz and Dot.
- [Svgbob Editor](https://ivanceras.github.io/svgbob-editor/) - Convert your ascii diagram scribbles into happy little SVG

## Visualization
- [Sparklines](https://en.wikipedia.org/wiki/Sparkline) are possible in plain-text (specifically these 8 characters: '▁▂▃▄▅▆▇█').
- [Tables-Generator](https://www.tablesgenerator.com/text_tables) lets you generate plain-text tables.

## Presentations


## Finance

Tools that let you manage finances, but keep your books in plain-text.

- \*[plain text accounting](https://plaintextaccounting.org/) - umbrella site for the plain text accounting community.
- [ledger](https://www.ledger-cli.org/) - Ledger is a powerful, double-entry accounting system that is accessed from the UNIX command-line
- [hledger](https://hledger.org/) - cross-platform accounting software for both power users and folks new to accounting.
- [beancount](http://furius.ca/beancount) - A double-entry bookkeeping computer language that lets you define financial transaction records in a text file, read them in memory, generate a variety of reports from them, and provides a web interface.
- [transity](https://github.com/feramhq/transity#list-of-features--todos) - A transaction-first plain-text account tool that uses YAML to store your transactions.
- ~~[plainbudget](https://galvez.github.io/plainbudget/) - Minimalist plaintext budgeting tool.~~

## Typesetting

Tools that let you create professional looking documents, but keep your books in plain-text.

- [LaTeX](http://www.texfaq.org/FAQ-latex)
- [SILE](https://sile-typesetter.org/what-is/) - a typesetting system written in Lua and using the HarfBuzz font shaper. It’s input syntax is somewhat inspired by LaTeX.
- [groff](https://gnu.org/software/groff/) - is a typesetting system that creates formatted output when given plain text mixed with formatting commands. Primarily used for man pages, it has been used for [books](https://rkrishnan.org/posts/2016-03-07-how-is-gopl-typeset.html) as well.
- [rinohtype](http://www.mos6581.org/rinohtype/master/) - a Python library that transforms a structured document into a professionally typeset PDF guided by a document template and style sheet.
- [pandoc](https://pandoc.org/) - If you need to convert files from one markup format into another, pandoc is your swiss-army knife.
- \*[Sustainable Authorship in Plain Text using Pandoc and Markdown](https://programminghistorian.org/en/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown)
- \*[Unicode Nearly Plain-Text Encoding of Mathematics](https://www.unicode.org/notes/tn28/UTN28-PlainTextMath-v3.pdf) - With a few conventions, Unicode1can encode manymathematical expressions in readable nearly plain text. Technically thisformat is a “lightly marked up format”; hence the use of “nearly”.
- [MathML](https://www.w3.org/Math/) - MathML is a low-level specification for mathematical and scientific content on the Web and beyond.
- \*[A list of MathML Tools](https://www.w3.org/wiki/Math_Tools)
- [AsciiDoctor](https://asciidoctor.org) - AsciiDoctor is a fast text processor & publishing toolchain for converting AsciiDoc to HTML5, DocBook & more.

## Miscellaneous

- [klog](https://github.com/jotaen/klog) - klog is a plain-text file format and a command line tool for time tracking.
- ~~[diffscuss](http://blog.hut8labs.com/introducing-diffscuss.html) - plain-text code review system.~~
- \*[The Plain Person’s Guide to Plain Text Social Science](https://plain-text.co/) [[PDF Version](https://kieranhealy.org/files/papers/plain-person-text.pdf)].
- \*[Improving Health Care with Plain-Text Medical Records and Git](https://www.gizra.com/content/plain-text-medical-records/)
- [Poor Man's Issue Tracker](https://github.com/driusan/PoormanIssueTracker) - a loosely defined set of conventions for using the filesystem as an issue tracker.
- [bug](https://github.com/driusan/bug) - bug writes code problem reports to plain text files as per the poor man's issue tracker conventions. Issues are stored as human readable plaintext files, they branch and merge along with the rest of your code, and you can resolve conflicts using your standard tools.

## Specification

- [OpenAPI Specification](https://swagger.io/specification/) - a standard, language-agnostic interface to RESTful APIs which allows both humans and computers to discover and understand the capabilities of the service without access to source code, documentation, or through network traffic inspection.
- \*[OpenAPI.Tools](https://openapi.tools/) - List of various tools that use the OpenAPI Specification including Convertors, Validators, Documentation, Mock Servers, SDK Generators, Text Editors and more.
- [MSON](https://github.com/apiaryio/mson) - A description format for describing data structures in common markup formats such as JSON, XML or YAML.

## Related
- See <https://plaintextproject.online/>.

## License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)
