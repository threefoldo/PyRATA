
Project development
****************************

Roadmap
============

Last report
-----------


TODO list following a decreasing priority order.
-------------------------------

* communication make tutorial to recognize NP and NP of NP, simple NE recognizer, Opinion mining or sentiment analysis
* api/engine module re implement match
* api/engine see the pattern search module and its facilities
* api/engine the b*b case exploration in semantic_analysis ; currently check only the next step, but should explore as many as iter !
* quality apply logging to semantic_step_parser.py + revise the method names
* quality test - dispatch merged group tests in individual tests
* quality clean deprecated verbosity argument compiled_pattern_re, syntactic* and semantic*, and may be test* ?
* quality revise the __main__ section of each py
* api/engine implement split, sub... in compiled_pattern_re module
* api/engine by default only the zero group is compared with eq and ne ; should be all the groups ?
* api/engine check negation of groups/alternatives
* api/engine what should be the normal behavior of an alternative embedded in a group e.g. pyrata_re.compile('raw="a" (pos~"JJ"* (pos="NNS"|pos="NNP"))+')
* api/engine implement backtracking on alternatives
* api/engine revise annotate, sub, extend, and update method signatures for working with kwargs
* quality test the chunk operator
* grammar think of an alternative as re implementatin of the chunk operator in the grammar.
* api/engine re implement insert, delete (sub with [] ; check), insert-to-the-leftmost (~ sub with reference)... 
* api/engine implement the position (from which word token position we start to search) and the search for annotate (not finditer) 
* communication structure the documentation http://www.sphinx-doc.org/en/stable/ ; publish on github pages
* quality evaluate performance http://www.marinamele.com/7-tips-to-time-python-scripts-and-control-memory-and-cpu-usage
* quality evaluate performance comparing to pattern and python 3 chunking (see the use example and show how to do similar)
* quality evaluate performance time `[pos="NNS" | pos="NNP"]`, `pos~"NN[SP]"` and 'pos~"(NNS|NNP)"' are equivalent forms. They may not have the same processing time.
* quality improve performance (memory and time) ; evaluate the possibility of doing the ply way to handle the debug/tracking mode
* grammar implement group reference so they can be matched later in the data with the \number special sequence
* grammar implement wildcards (so far handled by a `'!b*'` in `'!b* b'`
* grammar does class atomic with non atomic contraint should be prefered to not step to adapt one single way of doing stuff: partofclassconstraint -> NOT classconstraint more than step -> NOT step ; but the latter is simpler so check if it is working as expected wi quantifier +!pos:"EX" = +[!pos:"EX"])
* grammar allow grammar with multiple rules (each rule should have an identifier... and its own groupindex)
* grammar move the python methods as grammar components
* grammar think about the context notion 
* api/engine implement lex.lex(reflags=re.UNICODE)
* communication developer make diagrams to explain process and relations between files
* quality test complex regex as value
* quality code handle the test case of error in the patterns
* quality code test re methods on Compiled regular expression objects 


