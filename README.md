# About

This is a fork of the VimRepress project, located at http://www.vim.org/scripts/script.php?script_id=3510.

VimBlog is a plugin for managing a Wordpress blog using Vim. There are many similar plugins, but most are no longer being developed.

## Requirements

- Vim 7.3+ with python 2.6/2.7 support 
- Python Environment matched wtih Vim's support 
- python-markdown/python-markdown2 installed 
- Wordpress 3.0.0 +

## Command Examples

Some commands list above contain special usage, example below may clearify them for you. 


    :BlogList             -  List 30 recent posts. 
    :BlogList page        -  List 30 recent pages. 
    :BlogList post 100    -  List 100 recent posts. 

    :BlogNew post         -  Write an new post. 
    :BlogNew page         -  Write an new page. 

    :BlogSave             -  Save (defautely published.) 
    :BlogSave draft       -  Save as draft. 

    :BlogPreview local    -  Preview page/post locally in your browser. 
    :BlogPreview publish  -  Same as `:BlogSave publish' with brower opened. 

    :BlogOpen 679 
    :BlogOpen http://your-first-blog.com/archives/679 
    :BlogOpen http://your-second-blog.com/?p=679 
    :BlogOpen http://your-third-blog.com/with-your-custom-permalink 

## Modifications

I have made a number of changes (hence the name change) to make it more functional for me, including the following:

- I removed the prompt for editing or deleting posts, and am using a command to skip those steps during blogging workflow (see below)
- I moved the post type from Markdown to HTML because I have Wordpress doing Markdown conversion on the server side

## Commands

I set up a few shortcuts that I use during day-to-day blogging:

-  <code>nnoremap <leader>b :BlogSave publish<CR></code>
### Credits

All credit to Pentie for creating VimRepress, which this is based on.
