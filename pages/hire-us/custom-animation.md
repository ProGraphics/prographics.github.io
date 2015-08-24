---
layout: page
title: "Custom Web Animation"
desc: "Custom Web Animation."
breadcrumb-base: documentation
permalink: "/custom-animation/"
---

Want some eye-catching animated content? Whether it's a web page header, electronic brouchure, presentation, kiosk, or display. We can do it for you.

Fill out the form below and let us know how we can help you. _Please be as descriptive as possible and include your budget_. 


<!-- Note :
   - You can modify the font style and form style to suit your website. 
   - Code lines with comments “Do not remove this code”  are required for the form to work properly, make sure that you do not remove these lines of code. 
   - The Mandatory check script can modified as to suit your business needs. 
   - It is important that you test the modified form before going live.-->
<div id='crmWebToEntityForm' style='width:600px;margin:auto;'>
   <META HTTP-EQUIV ='content-type' CONTENT='text/html;charset=UTF-8'>
   <form action='https://crm.zoho.com/crm/WebToLeadForm' name=WebToLeads1631006000000085041 method='POST' onSubmit='javascript:document.charset="UTF-8"; return checkMandatory()' accept-charset='UTF-8'>

	 <!-- Do not remove this code. -->
	<input type='text' style='display:none;' name='xnQsjsdp' value='4ee271b6c2cd432ceb971a6c2bf0b720c48c59cb80c97be50d1a891be1306111'/>
	<input type='hidden' name='zc_gad' id='zc_gad' value=''/>
	<input type='text' style='display:none;' name='xmIwtLD' value='48da0bc0b512742cb8b14d7fac104d94122d44dcc264ec954b1910f8ef4981b7'/>
	<input type='text' style='display:none;'  name='actionType' value='TGVhZHM='/>

	<input type='text' style='display:none;' name='returnURL' value='http&#x3a;&#x2f;&#x2f;pro.graphics&#x2f;request-received&#x2f;' /> 
	 <!-- Do not remove this code. -->
	<style>
		tr , td { 
			padding:6px;
			border-spacing:0px;
			border-width:0px;
			}
	</style>
	<table style='width:600px;background-color:white;color:black'>

	<tr><td colspan='2' style='text-align:left;color:black;font-family:Arial;font-size:14px;'><strong>Custom Animation Request</strong></td></tr>

	<tr><td  style='nowrap:nowrap;text-align:right;font-size:12px;font-family:Arial;width:200px;'>First Name<span style='color:red;'>*</span></td><td style='width:250px;' ><input type='text' style='width:250px;'  maxlength='40' name='First Name' /></td></tr>

	<tr><td  style='nowrap:nowrap;text-align:right;font-size:12px;font-family:Arial;width:200px;'>Last Name<span style='color:red;'>*</span></td><td style='width:250px;' ><input type='text' style='width:250px;'  maxlength='80' name='Last Name' /></td></tr>

	<tr><td  style='nowrap:nowrap;text-align:right;font-size:12px;font-family:Arial;width:200px;'>Company<span style='color:red;'>*</span></td><td style='width:250px;' ><input type='text' style='width:250px;'  maxlength='100' name='Company' /></td></tr>

	<tr><td  style='nowrap:nowrap;text-align:right;font-size:12px;font-family:Arial;width:200px;'>Email<span style='color:red;'>*</span></td><td style='width:250px;' ><input type='text' style='width:250px;'  maxlength='100' name='Email' /></td></tr>

	<tr><td  style='nowrap:nowrap;text-align:right;font-size:12px;font-family:Arial;width:200px;'>Phone</td><td style='width:250px;' ><input type='text' style='width:250px;'  maxlength='30' name='Phone' /></td></tr>

	<tr><td  style='nowrap:nowrap;text-align:right;font-size:12px;font-family:Arial;width:200px;'>Website</td><td style='width:250px;' ><input type='text' style='width:250px;'  maxlength='255' name='Website' /></td></tr>

	<tr><td  style='nowrap:nowrap;text-align:right;font-size:12px;font-family:Arial;width:200px;'>Description<span style='color:red;'>*</span> </td><td> <textarea name='Description' maxlength='1000' style='width:250;'></textarea></td></tr>

	<tr><td colspan='2' style='text-align:center; padding-top:15px;'>
		<input style='font-size:12px;color:#131307' type='submit' value='Submit' />
		<input type='reset' style='font-size:12px;color:#131307' value='Reset' />
	    </td>
	</tr>
   </table>
	<script>
 	  var mndFileds=new Array('Company','First Name','Last Name','Email','Description');
 	  var fldLangVal=new Array('Company','First Name','Last Name','Email','Description');

 	  function checkMandatory() {
		var name='';
		var email='';
		for(i=0;i<mndFileds.length;i++) {
		  var fieldObj=document.forms['WebToLeads1631006000000085041'][mndFileds[i]];
		  if(fieldObj) {
			if (((fieldObj.value).replace(/^\s+|\s+$/g, '')).length==0) {
			  alert(fldLangVal[i] +' cannot be empty'); 
   	   	  	  fieldObj.focus();
   	   	  	  return false;
			}  else if(fieldObj.nodeName=='SELECT') {
  	   	   	 if(fieldObj.options[fieldObj.selectedIndex].value=='-None-') {
				alert(fldLangVal[i] +' cannot be none'); 
				fieldObj.focus();
				return false;
			   }
			} else if(fieldObj.type =='checkbox'){
 	 	 	 if(fieldObj.checked == false){
				alert('Please accept  '+fldLangVal[i]);
				fieldObj.focus();
				return false;
			   } 
			 } 
			 try {
			     if(fieldObj.name == 'Last Name') {
				name = fieldObj.value;
 	 	 	    }
			} catch (e) {}
		    }
		}
		 try {
		    if($zoho) {
			var LDTuvidObj = document.forms['WebToLeads1631006000000085041']['LDTuvid'];
			if(LDTuvidObj) {
  	  	 	    LDTuvidObj.value = $zoho.salesiq.visitor.uniqueid();
			}
			var firstnameObj = document.forms['WebToLeads1631006000000085041']['First Name'];
			if(firstnameObj) {
			     name = firstnameObj.value +' '+name;
			}
			$zoho.salesiq.visitor.name(name);
			var emailObj = document.forms['WebToLeads1631006000000085041']['Email'];
			if(emailObj) {
			     email = emailObj.value;
			     $zoho.salesiq.visitor.email(email);
			}
		    }
		} catch(e) {}
	     }
	   </script>
	</form>
</div>
