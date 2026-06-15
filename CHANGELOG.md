# Release notes

<!-- do not remove -->

## 0.0.52

### Bugs Squashed

- Move `__type` metadata injection from `finish_displayhook` to `write_format_data` ([#53](https://github.com/AnswerDotAI/ipykernel-helper/issues/53))


## 0.0.51

### New Features

- Wrap HTML output of dataframe-like objects in prose div ([#52](https://github.com/AnswerDotAI/ipykernel-helper/issues/52))


## 0.0.50

### New Features

- Use quad backticks ([#51](https://github.com/AnswerDotAI/ipykernel-helper/issues/51))


## 0.0.49

### New Features

- Wrap all markdown output in prose div via DisplayFormatter patch ([#50](https://github.com/AnswerDotAI/ipykernel-helper/issues/50))


## 0.0.47

### New Features

- Add `call_tool` helper for invoking funcs with coerced inputs ([#49](https://github.com/AnswerDotAI/ipykernel-helper/issues/49))


## 0.0.46

### Bugs Squashed

- fix `_await_cell_magic` if await inside code ([#48](https://github.com/AnswerDotAI/ipykernel-helper/issues/48))


## 0.0.45

### New Features

- Add `_safe_sig` helper to gracefully handle unintrospectable function signatures ([#47](https://github.com/AnswerDotAI/ipykernel-helper/issues/47))


## 0.0.44

### New Features

- Avoid double-await in `_await_cell_magic` by skipping lines already prefixed with await ([#46](https://github.com/AnswerDotAI/ipykernel-helper/issues/46))


## 0.0.43

### New Features

- In `finish_displayhook` add `__type` metadata ([#45](https://github.com/AnswerDotAI/ipykernel-helper/issues/45))


## 0.0.42

### Bugs Squashed

- Refactor `ranked_complete` to use explicit attrs in dict2obj instead of dynamic dir() lookup ([#44](https://github.com/AnswerDotAI/ipykernel-helper/issues/44))


## 0.0.41

### New Features

- Patch inspect.getfile to ensure return value is always a str ([#42](https://github.com/AnswerDotAI/ipykernel-helper/issues/42))


## 0.0.38

### New Features

- Add workaround for `structured_traceback` bug ([#41](https://github.com/AnswerDotAI/ipykernel-helper/issues/41))


## 0.0.37

### New Features

- Add dynamic signature help with `_sig_dyn` fallback and `_param_idx` tokenizer ([#40](https://github.com/AnswerDotAI/ipykernel-helper/issues/40))


## 0.0.36

### New Features

- Add `maybe_await` ([#39](https://github.com/AnswerDotAI/ipykernel-helper/issues/39))


## 0.0.35

### Bugs Squashed

- return None in repr ([#38](https://github.com/AnswerDotAI/ipykernel-helper/issues/38))


## 0.0.34

### New Features

- Truncate large non-str display obj reprs ([#37](https://github.com/AnswerDotAI/ipykernel-helper/issues/37))


## 0.0.33

### New Features

- Add `__repr__` to DisplayObject for readable display of data/url/filename ([#36](https://github.com/AnswerDotAI/ipykernel-helper/issues/36))


## 0.0.32

### New Features

- Add @llmtool to `read_gh_repo`/`read_url`, wrap Markdown repr in prose div, export `read_gh_repo` in extension ([#35](https://github.com/AnswerDotAI/ipykernel-helper/issues/35))


## 0.0.31

### New Features

- Add async cell magic support with automatic FT→HTML conversion ([#31](https://github.com/AnswerDotAI/ipykernel-helper/issues/31))

### Bugs Squashed

- improve eval expr error msg ([#29](https://github.com/AnswerDotAI/ipykernel-helper/pull/29)), thanks to [@RensDimmendaal](https://github.com/RensDimmendaal)


## 0.0.29

### New Features

- Support dotted names in `get_schemas` for object attribute access ([#30](https://github.com/AnswerDotAI/ipykernel-helper/issues/30))


## 0.0.28

### New Features

- Add eval expr ([#28](https://github.com/AnswerDotAI/ipykernel-helper/pull/28)), thanks to [@RensDimmendaal](https://github.com/RensDimmendaal)

### Bugs Squashed

- Fix UTF-8 encoding detection in `scrape_url` ([#27](https://github.com/AnswerDotAI/ipykernel-helper/pull/27)), thanks to [@ncoop57](https://github.com/ncoop57)


## 0.0.26

### New Features

- Improve `?` output formatting: wrap docstring in code block, optimize `info_dict` retrieval ([#26](https://github.com/AnswerDotAI/ipykernel-helper/issues/26))


## 0.0.25

### New Features

- Use docments text for info ([#25](https://github.com/AnswerDotAI/ipykernel-helper/issues/25))


## 0.0.22

### New Features

- Use `sig_source` ([#24](https://github.com/AnswerDotAI/ipykernel-helper/issues/24))


## 0.0.21

### New Features

- Use `skip_hidden` ([#23](https://github.com/AnswerDotAI/ipykernel-helper/issues/23))


## 0.0.19

### New Features

- Use new evalable param ([#22](https://github.com/AnswerDotAI/ipykernel-helper/issues/22))


## 0.0.18

### New Features

- Handle gh URLs ([#21](https://github.com/AnswerDotAI/ipykernel-helper/issues/21))


## 0.0.17

### New Features

- Add `fix_editable_priority` ([#20](https://github.com/AnswerDotAI/ipykernel-helper/issues/20))


## 0.0.16

### Bugs Squashed

- fix escape sequence in md img alt text ([#17](https://github.com/AnswerDotAI/ipykernel-helper/pull/17)), thanks to [@KeremTurgutlu](https://github.com/KeremTurgutlu)


## 0.0.15

### New Features

- enhance read_url ([#15](https://github.com/AnswerDotAI/ipykernel-helper/pull/15)), thanks to [@RensDimmendaal](https://github.com/RensDimmendaal)


## 0.0.14

### New Features

- add literal option to `get_vars` and fallback to str ([#14](https://github.com/AnswerDotAI/ipykernel-helper/pull/14)), thanks to [@KeremTurgutlu](https://github.com/KeremTurgutlu)


## 0.0.13

### Bugs Squashed

- fix `read_url` for non-html content ([#11](https://github.com/AnswerDotAI/ipykernel-helper/pull/11)), thanks to [@KeremTurgutlu](https://github.com/KeremTurgutlu)


## 0.0.12

### New Features

- Use cloudscraper ([#10](https://github.com/AnswerDotAI/ipykernel-helper/issues/10))


## 0.0.11

### New Features

- Read whole section when using anchor fragment in `read_url` ([#9](https://github.com/AnswerDotAI/ipykernel-helper/issues/9))


## 0.0.10

### New Features

- Add `_get_info`; improve `read_url` ([#8](https://github.com/AnswerDotAI/ipykernel-helper/issues/8))


## 0.0.7

### New Features

- Add `read_url` ([#7](https://github.com/AnswerDotAI/ipykernel-helper/issues/7))


## 0.0.6

### New Features

- Optional `data` for `run_cmd` ([#5](https://github.com/AnswerDotAI/ipykernel-helper/issues/5))


## 0.0.5

### New Features

- Add `run_cmd()` and transient() ([#4](https://github.com/AnswerDotAI/ipykernel-helper/issues/4))


## 0.0.4

### New Features

- Make it an extension ([#3](https://github.com/AnswerDotAI/ipykernel-helper/issues/3))


## 0.0.3

### New Features

- Move helpers into ipython terminal superclass ([#2](https://github.com/AnswerDotAI/ipykernel-helper/issues/2))


## 0.0.2

- more helpers


## 0.0.1

- init working version

