> {textInput}

```html
<div class="form-group">
    <input type="text" class="form-control">
</div>
```

> {textInput id='username' value='my-user-name'}

```html
<div class="form-group">
    <input type="text" class="form-control" id="username" name="username" value="my-user-name">
</div>
```

> {textInput name='login[username]'}

```html
<div class="form-group">
    <input type="text" class="form-control" id="loginUsername" name="login[username]">
</div>
```

> {dateInput format='datetime'}

> {dateInput format='date' type='jalali' value='2020-02-15'}

> {textareaInput} hello world! {/textareaInput}

> {selectInput value='system' options=['all', 'system']}

> {select2Input value='system' options=$options}

> {radioInput id='sex' label='male'}

> {radioListInput options=$options}

> {submitButton value='submit'}

> {info icon='fa fa-times'} add some text for input... {info}

> {datatable data=$data}

> {datatable url='@webroot/modules/data.php'}

{datatable url='@modulelink/data.php'}
    {col title='id'}{$id}{/col}
    {col title='fullname'}{$firstname|trim} {$lastname|trim}{/col}
    {col title='link'}{$ticketId|link:'@modulelink&action=' + $ticketId}{/col}
{/datatable}

{searchPanel}
    {textInput id='username'}
    {dateInput format='datetime'}
    {select2Input value='system' options=$options}
{/searchPanel}

> {msg type='warning'} some error happened! {msg}

> {msg key='issupport'}

> {alert type='success'} data saved successfully. {/alert}

> {alert key='issupport'}

> {$var|link}

> {$webRoot}

> {$manager}

> {$moduleLink}

> {$clientModuleLink}

{modal id='createPage'}
    {title}some title{/title}
    {body}some text...{/body}
    {footer}{button}{/footer}
{/modal}
