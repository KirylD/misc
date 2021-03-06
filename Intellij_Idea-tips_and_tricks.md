# Live Templates

* Logs a value to LOGGER.info
  * Template text 
    ```batch
    $LOGGER$.info("$EXPR_COPY$ = {}", $EXPR$); 
    ```
* Slf4j Logger
  * Template text 
    ```batch
    private static final org.slf4j.Logger LOGGER = org.slf4j.LoggerFactory.getLogger($CLASS$.class);
    ```
* Log4j Logger
  * Template text 
    ```batch
    private static final org.apache.logging.log4j.Logger LOG = org.apache.logging.log4j.LogManager.getLogger($CLASS$.class);
    ```
* Surround XML with region marker
  * Template text 
    ```batch
    <!--region $DESCRIPTION$-->
    $SELECTION$
    <!--endregion-->
    ```
* Variables:

| Name | Expression | Default Value | Skip if defined |
| --- | --- | --- | --- |
| LOGGER | variableOfType(“Logger”) | LOGGER | [] |
| EXPR | variableOfType(“”) | “expr” | [] |
| EXPR_COPY | escapeString(EXPR) | | [x] |
| CLASS | className() | | [] |
| DESCRIPTION |  | “Description” | [] |

# Optimized setting for Intellij Idea:

## Clean the view
* *Navigation Bar* - OFF. This is really useful option to save space. You can always view navigation bar by 'Alt+home'.
* *Breadcrumbs* - deactivate it to save space, cause it has no sense in *.java files.
* *Highlight usages of element at caret*(Settings > General) - it is rather irritating option which is active by default. You can always highlight the element under the caret by 'Shift+Ctrl+F7'.
* *Editor > Color scheme > General: section 'Editor', property 'Caret row'* - deactivate the checkbox 'Background'.
* *Editor > Color scheme > Language Defaults, property 'Semantic highlighting'* - activate the checkbox 'Semantic highlighting'
 
## Must-have plugins
* *Findbugs-IDEA* - provides static byte code analysis to look for bugs in Java code from within IntelliJ IDEA.
* *Checkstyle-IDEA* - provides both real-time and on-demand scanning of Java files with CheckStyle from within IDEA.
* *Lombok* - a plugin that adds first-class support for Project Lombok
* *JMH Plugin* - a plugin for generating and running JMH benchmarks from your IDE
* *.ignore* - is a plugin for .gitignore (Git), .hgignore (Mercurial), .npmignore (NPM), .dockerignore (Docker), .chefignore (Chef), .cvsignore (CVS), .bzrignore (Bazaar), .boringignore (Darcs), .mtn-ignore (Monotone), ignore-glob (Fossil), .jshintignore (JSHint), .tfignore (Team Foundation), .p4ignore (Perforce), .prettierignore (Prettier), .flooignore (Floobits), .eslintignore (ESLint), .cfignore (Cloud Foundry), .jpmignore (Jetpack), .stylelintignore (StyleLint), .stylintignore (Stylint), .swagger-codegen-ignore (Swagger Codegen), .helmignore (Kubernetes Helm), .upignore (Up), .prettierignore (Prettier), .ebignore (ElasticBeanstalk) files in your project. 
* *Grep Console* - grep, tail, filter, highlight... everything you need for a console. Also can highlight the editor - nice for analyzing logs.
* *Key promoter* - helps you to learn essential shortcuts while you are working. 
* *Maven helper* -a must have plugin for working with Maven.
* *BashSupport* - it adds Bash language support for the IntelliJ platform.
* *InnerBuilder* - adds a Builder action to the Generate menu (Alt+Insert) which generates an inner builder class as described in Effective JavaProvideProvides intelligent spelling and grammar checks for text that you write in the IDE.s intelligent spelling and grammar checks for text that you write in the IDE.
Supports run configurations, syntax highlighting, rename refactoring, documentation lookup, inspections, quickfixes and much more.
* *Database Navigator* - database development, scripting and navigation tool. It adds extensive database development and maintenance capabilities to the IntelliJ IDEA development environment and related products
* *Grazie* - provides intelligent spelling and grammar checks for text that you write in the IDE.
* *RegexpTester* - Regular Expression Tester for IntelliJ IDEA. Allows you to experiment with Java regular expressions in a dynamic environment.
* *Intend RainBow* - a simple extension to make indentation more readable. This extension colorizes the indentation in front of your text alternating four different colors on each step.
* *Rainbow Brackets* - a simple extension to make the usage of brakets more readable.
* *IDEA Mind Map* - brain storming and task decomposition
* *Power Mode II* - for epic coding.
* *Code Screenshot* - selects a code and press a hot-key (Ctrl+Alt+Shift+A by default) to copy it as the image (make a screenshot).
Default hot-key can be changed in Settings|Keymap (search for "Copy as image" action)
* *TweetCode* - share code fragments in twitter
* *IdeaTweet* - share code fragments in twitter

## Good talks
- [x] [Be More Productive With IntelliJ IDEA by Trisha Gee](https://www.youtube.com/watch?v=CmPJzEqFS4s)
- [x] [Trisha Gee - IntelliJ IDEA 2019.1. Structural Search and Replace](https://www.youtube.com/watch?v=fIPr_ANBpFk)
- [x] [Тагир Валеев — Атомарный рефакторинг в IntelliJ IDEA: прогибаем IDE под себя](https://www.youtube.com/watch?v=C5eD-K8AO3o&list=PLVe-2wcL84b_fBL9xJTxkEBtvCKfRGEV1&index=5)
- [x] ['Zen Habits of using IntelliJ IDEA by Victor Kropp'](https://www.youtube.com/watch?v=MZge92bbU7E).


# Top keybindings in Intellij Idea
| Keybind | What it does |
| ------------- | ------------- |
| **Alt+Up/Down** | Jump to next method |
| **Alt+Left/Right** | Switch to previous/next tab  |
| **Ctrl+Alt+Left/Right** | Go back/forward location  |
| **Shift+Alt+Up/Down** | Move code  |
| **Ctrl+F4** |Close current tab |
| **Ctrl+Alt+L** |Reformat selected code |
| **Ctrl+Alt+O** |Organise Imports |
| **Alt+Enter** | Show action intentions  |
| **Ctrl+Space** | Basic code completion  |
| **Ctrl+Shift+Space** | Complete current statement  |
| **Ctrl+B** | Go to declaration |
| **Ctrl+P** | Parameter info |
| **Ctrl+D** | Duplicate line |
| **Ctrl+X** | Cut line/highlighted |
| **Ctrl+F** | Search in current file |
| **Ctrl+R** | Replace in current file |
| **Ctrl+Shift+F** | Find in path |
| **Ctrl+Shift+R** | Replace in path |
| **Double Shift** | Search everywhere |
| **Double Ctrl** | Run anything |
| **Ctrl+Shift+N** | Search classes/files/symbols/actions |
| **Alt+Insert** | Generate code (can be done in multiple views) |
| **Ctrl+Alt+M** | Extract method(with code highlighted)  |
| **Ctrl+Alt+V** | Extract variable(with code highlighted)  |
| **Alt+F8** | Open evaluation window(in debug)  |
| **Ctrl+/** | Comment code |
| **Ctrl+Shift+/** | Comment block code |
| **Shift+F6** | Rename |
| **Shift+F9** | Run in debug |
| **Shift+F10** | Run |
| **Alt+F9** | Continue execution and stop at cursor(in debug) |
| **Alt+F10** | Go to where execution stopped(in debug) |
| **F9** | Resume Program(in debug) |
| **F7** | Step into(in debug) |
| **F8** | Step over(in debug) |
| **Ctrl+F8** | Add breakpoint |
| **Alt+F7** | Find all usages  |
| **Ctrl+Alt+F7** | Show usages  |
| **Ctrl+Up/Down** | Move view  |
| **Alt+1** | Show/hide *Project* explorer  |
| **Alt+7** | Show/hide *Structure*  |
| **Alt+Insert** | Create new. F.e. `Alt+1, Alt+Insert` will create a new file.  |
| **Ctrl+E** | Show dialog *Recent Files*  |
| **Ctrl+Shift+E** | Show dialog *Recent Locations*  |
| **Ctrl+Shift+V** | Paste from recent clipboards  |
| **Ctrl+Alt+S** | Settings  |
| **Ctrl+Alt+Shift+S** | Project Settings  |
| **Ctrl+T** | Update `Project`  |
| **Ctrl+K** | Commit changes window  |
| **Ctrl+O** | Override methods  |
| **Ctrl+I** | Implement methods  |
| **Alt+J** | Select next occurence  |
| **Ctrl+Alt+T** | Surround with  |
| **Ctrl+Shift+Alt+T** | Refactor this  |
 
