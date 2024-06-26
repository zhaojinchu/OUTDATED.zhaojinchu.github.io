---
layout: cv
title: CV
---


# Curriculum Vitæ
<br/>

<div id="pdf-container" style="position: relative; width: 100%; height: 0; padding-bottom: 0;">
    <object id="pdf-object" data="{{ site.baseurl }}/assets/files/cv.pdf" type="application/pdf" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;">
        <p>Your browser does not support PDFs. 
            <a href="{{ site.baseurl }}/assets/files/cv.pdf">Download the PDF</a>.
        </p>
    </object>
</div>

<script>
    document.addEventListener("DOMContentLoaded", function() {
        var pdfContainer = document.getElementById('pdf-container');
        var pdfObject = document.getElementById('pdf-object');

        // PDF page height in pixels
        var pdfPageHeight = 1122; // Adjust this value based on your PDF page height
        pdfContainer.style.height = pdfPageHeight + 'px';
        pdfObject.style.height = '100%';
    });
</script>

{% include contact.html %}

