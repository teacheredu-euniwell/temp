<!--
version:  2024.10.24

author:   TEST

email:    teacheredu.euniwell@uni-konstanz.de

comment:  TEST
          
logo:     https://raw.githubusercontent.com/teacheredu-euniwell/temp/6ab0c53dcc55e15144f0b5816727648a088727b8/media/ch0/CC_BY-SA_icon.svg

icon:     https://raw.githubusercontent.com/teacheredu-euniwell/temp/6ab0c53dcc55e15144f0b5816727648a088727b8/media/ch0/CC_BY-SA_icon.svg

language: en

narrator: English Female

mode:     Textbook
dark:     false

date:     24/10/2024

attribute: TEST

  ![CC-BY-SA](media/CC-BY-SA-icon.svg)

translateWithGoogle: true

script:  https://h5p.org/sites/all/modules/h5p/library/js/h5p-resizer.js

@h5p_embed: @h5p_embed_(@uid,@0)

@h5p_embed_
<iframe id="h5p_@0" style="width:100%;" srcdoc='<!DOCTYPE html><html lang="de"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1.0"><style>body{display:flex;justify-content:center;align-items:center;height:100vh;margin:0;background-color:#f0f0f0}.loader{border:16px solid #f3f3f3;border-top:16px solid #3498db;border-radius:50%;width:80px;height:80px;animation:spin 2s linear infinite}@keyframes spin{0%{transform:rotate(0deg)}100%{transform:rotate(360deg)}}</style></head><body><div class="loader"></div></body></html>'></iframe>
<script run-once>
fetch('@1')
    .then(response => {
        if (!response.ok) {
            throw new Error('Netzwerkantwort war nicht ok ' + response.statusText);
        }
        return response.text(); // Abruf als Text
    })
    .then(htmlText => {
        document.getElementById('h5p_@0').srcdoc = htmlText;
        send.lia("LIA: stop");
    })
    .catch(error => {
        console.error('Es gab ein Problem mit dem Abruf: ', error);
        send.error("LIA: stop");
    });

"LIA: wait"
</script>
@end

-->


# TEST

Subsubfolder ![alt text](media/ch0/CC-BY-SA-icon.svg)

Subfolder ![alt text](media/CC-BY-SA-icon.svg)

Mainfolder ![alt text](CC-BY-SA-icon.svg)


Neuer Eintrag

H5P
===

iframe
---

[text](media/ch0/bronfenbrenner-dragdrop.html)

<iframe src=https://github.com/teacheredu-euniwell/temp/raw/refs/heads/main/media/ch0/bronfenbrenner-dragdrop.html width="958" height="687" frameborder="0" allowfullscreen="allowfullscreen" title="Fends Social Systems Interaction (Drag &amp; Drop)"></iframe><script src="https://euniwell.de.cool/wp-content/plugins/h5p/h5p-php-library/js/h5p-resizer.js" charset="UTF-8"></script>

H5P Embed
---

<!--
persistent: true
-->
@[h5p_embed](media/ch0/bronfenbrenner-dragdrop.html)