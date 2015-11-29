---
layout: docs
title: Reserved Variable Names
short_title: Reserved Names
---

The following variables are set internally by **docassemble**.  If you
try to use these reserved names for your own purposes, you will
experience errors or unexpected results.

* `_internal`: used internally by **docassemble** for various
  purposes, including keeping track of the progress bar, storing the
  answers to multiple-choice questions, and tracking which questions
  have already been answered.
* `current_info`: a dictionary available to the interview code that
  contains some useful information about the interview and the current
  user.  It is pre-set by **docassemble** on every page load.
* `i`: used as an iterator when [generic objects] are defined.
* `role`: used to store the role of the current user for purposes of
  the [roles] system.
* `track_location`: used to indicate whether the web app should
  attempt to determine the user's latitude and longitude and make it
  available in `current_info`.
* `role_event`: a special variable that is used as part of the [roles]
  system.
* `role_needed`: a special variable that is used as part of the [roles]
  system.
* `url_args`: a dictionary available to interview code that contains
  values encoded in the URL with which the interview was initially
  loaded.
* `x`: used as a reference to the underlying object when
  [generic objects] are defined.

If you include the `basic-questions.yml` file from `docassemble.base`,
the list of reserved names expands to the following:

* `Asset`
* `Case`
* `ChildList`
* `Court`
* `DAFileCollection`
* `DAFileList`
* `DAFile`
* `DAList`
* `DATemplate`
* `Document`
* `Expense`
* `FinancialList`
* `Income`
* `Individual`
* `Jurisdiction`
* `LegalFiling`
* `PartyList`
* `PeriodicFinancialList`
* `PeriodicValue`
* `Person`
* `RoleChangeTracker`
* `Value`
* `_internal`
* `advocate`
* `blank_signature`
* `capitalize`
* `case`
* `client`
* `comma_and_list`
* `comma_list`
* `court`
* `currency`
* `current_info`
* `cutoff_date`
* `force_ask`
* `get_info`
* `get_language`
* `get_locale`
* `i`
* `indefinite_article`
* `interview_url`
* `jurisdiction`
* `need`
* `nice_number`
* `noun_plural`
* `ordinal`
* `ordinal_number`
* `period_list`
* `pleading`
* `process_action`
* `role`
* `role_event`
* `selections`
* `send_email`
* `set_info`
* `set_language`
* `set_locale`
* `space_to_underscore`
* `spouse`
* `title_case`
* `today`
* `update_info`
* `url_action`
* `url_args`
* `url_of`
* `us`
* `user_lat_lon`
* `user_understands_how_to_use_signature_feature`
* `user_understands_no_attorney_client_relationship`
* `user`
* `verb_past`
* `verb_present`
* `word`
* `words`
* `x`
* `your`

In addition, [Python] uses the following names as part of the
language.  If you use any of these as your own variable names, you may
encounter an error or an unexpected problem.

* `ArithmeticError`
* `AssertionError`
* `AttributeError`
* `BaseException`
* `BufferError`
* `BytesWarning`
* `DeprecationWarning`
* `EOFError`
* `Ellipsis`
* `EnvironmentError`
* `Exception`
* `False`
* `FloatingPointError`
* `FutureWarning`
* `GeneratorExit`
* `IOError`
* `ImportError`
* `ImportWarning`
* `IndentationError`
* `IndexError`
* `KeyError`
* `KeyboardInterrupt`
* `LookupError`
* `MemoryError`
* `NameError`
* `None`
* `NotImplementedError`
* `NotImplemented`
* `OSError`
* `OverflowError`
* `PendingDeprecationWarning`
* `ReferenceError`
* `RuntimeError`
* `RuntimeWarning`
* `StandardError`
* `StopIteration`
* `SyntaxError`
* `SyntaxWarning`
* `SystemError`
* `SystemExit`
* `TabError`
* `True`
* `TypeError`
* `UnboundLocalError`
* `UnicodeDecodeError`
* `UnicodeEncodeError`
* `UnicodeError`
* `UnicodeTranslateError`
* `UnicodeWarning`
* `UserWarning`
* `ValueError`
* `Warning`
* `WindowsError`
* `ZeroDivisionError`
* `__debug__`
* `__doc__`
* `__import__`
* `__name__`
* `__package__`
* `_`
* `abs`
* `all`
* `and`
* `any`
* `apply`
* `as`
* `assert`
* `basestring`
* `bin`
* `bool`
* `break`
* `buffer`
* `bytearray`
* `bytes`
* `callable`
* `chr`
* `class`
* `classmethod`
* `cmp`
* `coerce`
* `compile`
* `complex`
* `continue`
* `copyright`
* `credits`
* `def`
* `del`
* `delattr`
* `dict`
* `dir`
* `divmod`
* `elif`
* `else`
* `enumerate`
* `eval`
* `except`
* `exec`
* `execfile`
* `exit`
* `file`
* `filter`
* `finally`
* `float`
* `for`
* `format`
* `from`
* `frozenset`
* `getattr`
* `global`
* `globals`
* `hasattr`
* `hash`
* `help`
* `hex`
* `id`
* `if`
* `import`
* `in`
* `input`
* `int`
* `intern`
* `is`
* `isinstance`
* `issubclass`
* `iter`
* `lambda`
* `len`
* `license`
* `list`
* `locals`
* `long`
* `map`
* `max`
* `memoryview`
* `min`
* `next`
* `not`
* `object`
* `oct`
* `open`
* `or`
* `ord`
* `pass`
* `pow`
* `print`
* `print`
* `property`
* `quit`
* `raise`
* `range`
* `raw_input`
* `reduce`
* `reload`
* `repr`
* `return`
* `reversed`
* `round`
* `set`
* `setattr`
* `slice`
* `sorted`
* `staticmethod`
* `str`
* `sum`
* `super`
* `try`
* `tuple`
* `type`
* `unichr`
* `unicode`
* `vars`
* `while`
* `with`
* `xrange`
* `yield`
* `zip`

In addition, you should never use a variable name that begins with an
underscore.  Although `_internal` is the only variable in the variable
store that begins with an underscore, the **docassemble** web app uses
names that begin with underscores to communicate information between
the browser and the server, and if your variable names conflict with
these names, you may experience errors or unexpected results.  These
internal names include:

* `_attachment_email_address`
* `_attachment_include_rtf`
* `_back_one`
* `_checkboxes`
* `_datatypes`
* `_email_attachments`
* `_files`
* `_question_number`
* `_question_name`
* `_save_as`
* `_success`
* `_the_image`
* `_tracker`

The following URL parameters have special meaning in **docassemble**.
All others are available for you to use and to retrieve with
[url_args].

* `i`: indicates the interview file to use
* `session`: indicates the key of the stored dictionary to use
* `action`: used by the `url_action` [function]
* `filename`: used for retrieving documents
* `question`: used for retrieving documents
* `format`: used for retrieving documents
* `index`: used for retrieving documents

[function]: {{ site.baseurl }}/docs/functions.html
[url_args]: {{ site.baseurl }}/docs/.html
[roles]: {{ site.baseurl }}/docs/roles.html
[generic objects]: {{ site.baseurl }}/docs/modifiers.html
[Python]: https://en.wikipedia.org/wiki/Python_%28programming_language%29