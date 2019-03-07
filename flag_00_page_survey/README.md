### Data Validation Vulnerability
##### [page_survey]('http://192.168.56.101/?page=survey')

###### Using JQuery to make a POST request and inject to page

```
        $.post("index.php?page=survey", { sujet: 2, valeur: 110 },
                function(a, c, d, e) {
                        $('body')[0].innerHTML = a;}
                                );
```

