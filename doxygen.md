###Required packages on Xubuntu
`sudo apt-get install doxygen doxygen-gui graphviz`

###Running the Wizard
`doxywizard`

###Config Items
`PROJECT_NAME` -> name of the project for which docs are being generated

`OUTPUT_DIRECTORY` -> path where the generated stuff will be placed

`OPTIMIZE_OUTPUT_FOR_C` -> set to true if the source is all in C

`BUILTIN_STL_SUPPORT` -> use doxygen's STL stuff instead of using it from tagfiles

`EXTRACT_ALL` -> set to YES to document stuff that doesn't have doxygen doc tags

`EXTRACT_PACKAGE` -> set to YES to document internal scope stuff

`EXTRACT_STATIC` -> set to YES to document file-level static stuff

`EXTRACT_LOCAL_CLASSES` -> set to YES to document classes defined in src files (useful for functors)

`SHOW_INCLUDE_FILES` -> set to NO to disable verbose printing of includes in the generated doc page

`INLINE_INFO` -> set to YES to see an [inline] annotation for inline functions

`SORT_BY_SCOPE_NAME` -> set to YES to sort by FQN, else sorts by class name only

`GENERATE_TODOLIST`/`GENERATE_TESTLIST`/`GENERATE_BUGLIST`/`GENERATE_DEPRECATEDLIST` -> set to NO to disable autogen of respective list

`INPUT` -> specifies files/dirs to parse

`FILE_PATTERNS` -> specifies filename pattern to look for when parsing

`RECURSIVE` -> set to YES to descend into subdirs of INPUT

`EXCLUDE` -> specifies dirs to exclude, paths either full or relative to INPUT. Separate multiple by space and line continuation with `\` (backslash)

`EXCLUDE_PATTERNS` -> specifies wildcarded patterns to exclude from INPUT (matches anywhere in path)

`SOURCE_BROWSER` -> set to YES to enable generation of src file list

`REFERENCED_BY_RELATION` -> set to YES to list all funcs referencing given func

`REFERENCES_RELATION` -> set to YES to list all tags being used by given func

`REFERENCES_LINK_SOURCE` -> set to YES to hyperlink the above two

`VERBATIM_HEADERS` -> set to NO to disable inclusion of header

`SEARCHENGINE` -> set to YES for searchbox with generated HTML

`CLASS_DIAGRAMS` -> set to YES to generate class diagrams with graphviz

`HAVE_DOT` -> set to YES to indicate dot tool (graphviz) is available for generating diagrams

`DOT_NUM_THREADS` -> set to 4 (number) indicating max. parallel dot instances to be created

`DOT_FONTSIZE` -> set to 12 (number) indicating font size for label text in generated diagrams

`CLASS_GRAPH` -> set to YES to generate inheritance diagrams

`COLLABORATION_GRAPH` -> set to YES to get class interdependencies

`UML_LOOK` -> set to YES to get UML-like diagrams for class etc

`INCLUDE_GRAPH`/`INCLUDED_BY_GRAPH` -> set to YES

`CALL_GRAPH`/`CALLER_GRAPH` -> set to YES

`GRAPHICAL_HIERARCHY`/`DIRECTORY_GRAPH` -> set to YES

`DOT_IMAGE_FORMAT` -> set to file extn for generated dot diagrams

`DOT_CLEANUP` -> delete intermediate dot files


