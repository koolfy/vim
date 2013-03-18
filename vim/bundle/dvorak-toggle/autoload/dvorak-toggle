" Quick Dvorak-layout toggle. 
" when toggled, you can use ctsr to move 
" when untoggled, ctsr will behave as expected by vim 
" 
" This code is under BSD licence, and the author doesn't even bother tell his identity.
 
let s:DvorakToggleState = 0
let s:DvorakToggleOldMap = 0
 
function! g:DvorakToggle () 
  if s:DvorakToggleState 
    :set langmap=s:DvorakToggleOldMap 
    let s:DvorakToggleState = 0 
  else  
    let g:DvorakToggleOldMap = &langmap 
    :set langmap=ctsrCTSRhjklHJKL;hjklHJKLctsrCTSR 
    let s:DvorakToggleState = 1 
  endif 
endfunction 
 
" use à or whatever you want. Make it easy to access though. 
nmap à :call g:DvorakToggle()<CR>
