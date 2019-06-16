# XAI
Zadania z Interpretowalnego Uczenia Maszynowego

Podsumowanie:
[Summary](BartlomiejKrzepkowskiPD10.pdf)


function appendPdf(id, url) {
    var $el = $('#'+id);
    // Check whether the browser supports displaying pdf files inline (ie. without downloading them)
    if (navigator && navigator.mimeTypes && navigator.mimeTypes['application/pdf']) {
        // You may add extra attributes (eg. to allow transparency) or style the iframe
        $el.html('<iframe src="'+url+'"></iframe>');
    } else {
        $el.html('<a href="'+url+'">Download file</a>');
    }
 }
