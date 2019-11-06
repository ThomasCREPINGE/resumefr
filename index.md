---
layout: cv
title: Thomas CREPINGE
---
# Thomas CREPINGE
Java Lead Developer

<div id="webaddress">
<a href="crepinge.thomas@gmail.com">crepinge.thomas@gmail.com</a>
</div>

<div id="content">
     <h3>Hello, this is a H3 tag</h3>

    <p>a pararaph</p>
</div>
<div id="editor"></div>
<button id="cmd">Generate PDF</button>

## Currently

Lead developer for Decathlon


### Specialized in

Java language, API REST architecture


## Education

`2007-2010`
__Lycée Voltaire de Wingles, Baccalauréat scientifique__

`2010-2016`
__Institut Supérieur d'Electronique et du Numérique.__


## Leasures


<!-- ### Footer

Last updated: November 2019 -->

<script>
    var doc = new jsPDF();
    var specialElementHandlers = {
        '#editor': function (element, renderer) {
            return true;
        }
    };

    $('#cmd').click(function () {
        doc.fromHTML($('#content').html(), 15, 15, {
            'width': 170,
                'elementHandlers': specialElementHandlers
        });
        doc.save('sample-file.pdf');
    });

    // This code is collected but useful, click below to jsfiddle link.
</script>


