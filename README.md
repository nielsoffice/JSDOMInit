# JSDOMInit
JS DOM init

```JS
jQuery(() => {
	
 const NielsOfficeHover = function( objectElem = {} ) {
	
  this.target = objectElem;	 
	 
 }	
 
 NielsOfficeHover.prototype.init = function() {
	
  let objectData = this.target;
  let __dataID   = objectData.ID;
	 
  jQuery(__dataID).bind('mouseenter', function() {
	 
     alert('Your cursor getting enter within HTML Element! ');
      
  });	
	 
 }	
 	
 // init 
 const NielsOffice = function( oe ) {
	
  const Success = new NielsOfficeHover( oe );
	Success.init();
 }
 
 // USAGE:
 NielsOffice({
	
   ID    : '#dataID',
   Class : 'Class-a'
	 
 });
 
});
```
