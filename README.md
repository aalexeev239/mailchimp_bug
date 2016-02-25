# mailchimp_bug
mailchimp bug

Image is linked either in html code, either in conditional comment for MS Outlook. Url in conditional comment is not processed while uploading to Mailchimp.

Source code:
```
<td background="./images/mario.jpg" bgcolor="#7bceeb" width="460" height="276" valign="top">
        <!--[if gte mso 9]>
        <v:rect xmlns:v="urn:schemas-microsoft-com:vml" fill="true" stroke="false" style="width:460px;height:276px;">
          <v:fill type="tile" src="./images/mario.jpg" color="#7bceeb" />
          <v:textbox inset="0,0,0,0">
        <![endif]-->
```

Upload bug.zip to MC: Templates > Create Template > Code Your Own > Import Zip.

```
 <td background="https://gallery.mailchimp.com/4bbc5ef81dbd2a87253a6b2f6/images/6fc18d6d-ec9e-487f-b85f-58cfd96f0d64.jpg" bgcolor="#7bceeb" width="460" height="276" valign="top">
        <!--[if gte mso 9]>
        <v:rect xmlns:v="urn:schemas-microsoft-com:vml" fill="true" stroke="false" style="width:460px;height:276px;">
          <v:fill type="tile" src="./images/mario.jpg" color="#7bceeb" />
          <v:textbox inset="0,0,0,0">
        <![endif]-->
```
