<script>
    let quote
    let author
    fetch('https://api.quotable.io/random?tags=education|happiness|inspirational|life|love|nature|science|technology|wisdom?maxLength=34').then( response => {
       return response.json()
    }).then(data => {
        quote = data.content
        author = data.author
    })
</script>

<div class="typewriter">
    <h2 style="color:dodgerblue;">{quote === undefined ? '' : quote}<span style="color:deepskyblue">&nbsp;-{author === undefined ? '' : author}</span></h2>
    <h2 style="color:mediumspringgreen;">Have an amazing time and a happy and long life.</h2>
    <h2 style="color:mediumslateblue;">Good bye and Thank you😊</h2>
</div>