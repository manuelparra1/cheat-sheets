# Hide Code - Jupyter Notebook

#### If you don't want to <br>`pip install` or `conda install` <br> jupyter notebook plugins/extensions

<br>

> Paste this code into notebook cell
> <br> and run as code

```python

from IPython.display import HTML

HTML('''<script>
code_show=true;
function code_toggle() {
 if (code_show){
 $('div.input').hide();
 } else {
 $('div.input').show();
 }
 code_show = !code_show
}
$( document ).ready(code_toggle);
</script>
<form action="javascript:code_toggle()"><input type="submit" value="Hide/Show: Raw Code"></form>''')

```
