# asyncomplete-gitcommit

Git commit message completion source for [asyncomplete.vim](https://github.com/prabirshrestha/asyncomplete.vim)

## Installing

```vim
Plug 'prabirshrestha/asyncomplete.vim'
Plug 'laixintao/asyncomplete-gitcommit'
```

## Register asyncomplete-gitcommit

```vim
au User asyncomplete_setup call asyncomplete#register_source({
    \ 'name': 'gitcommit',
    \ 'whitelist': ['gitcommit'],
    \ 'priority': 10,
    \ 'completor': function('asyncomplete#sources#gitcommit#completor')
    \ })
```

## TODO

- [ ] Support close github issues and PR;
- [ ] Read commit logs
