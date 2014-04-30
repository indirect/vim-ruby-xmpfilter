Use xmpfilter directly from vim, with no external (e.g. gem) dependencies

![Example](https://github.com/t9md/t9md/blob/master/img/vim-ruby-xmpfilter_anime.gif?raw=true)

## Installation (with Pathogen)

```
cd ~/.vim/bundle
git clone https://github.com/indirect/vim-ruby-xmpfilter.git
```

See, no dependencies!

## Usage

vim-ruby-xmpfilter doesn't provide a default keymap.
Add something like this to your `.vimrc`.

### vim (<leader>m & <leader>r)

    autocmd FileType ruby nmap <buffer> <leader>m <Plug>(xmpfilter-mark)
    autocmd FileType ruby xmap <buffer> <leader>m <Plug>(xmpfilter-mark)
    autocmd FileType ruby imap <buffer> <leader>m <Plug>(xmpfilter-mark)

    autocmd FileType ruby nmap <buffer> <leader>r <Plug>(xmpfilter-run)
    autocmd FileType ruby xmap <buffer> <leader>r <Plug>(xmpfilter-run)
    autocmd FileType ruby imap <buffer> <leader>r <Plug>(xmpfilter-run)

### MacVim (⌥M & ⌥R)

To use the option key as as meta in MacVim, run `:set macmeta`.

    autocmd FileType ruby nmap <buffer> <M-m> <Plug>(xmpfilter-mark)
    autocmd FileType ruby xmap <buffer> <M-m> <Plug>(xmpfilter-mark)
    autocmd FileType ruby imap <buffer> <M-m> <Plug>(xmpfilter-mark)

    autocmd FileType ruby nmap <buffer> <M-r> <Plug>(xmpfilter-run)
    autocmd FileType ruby xmap <buffer> <M-r> <Plug>(xmpfilter-run)
    autocmd FileType ruby imap <buffer> <M-r> <Plug>(xmpfilter-run)
