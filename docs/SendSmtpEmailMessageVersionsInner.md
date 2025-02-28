# SendSmtpEmailMessageVersionsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**to** | [**Vec<models::SendSmtpEmailToInner>**](sendSmtpEmail_to_inner.md) | List of email addresses and names (_optional_) of the recipients. For example, **[{\"name\":\"Jimmy\", \"email\":\"jimmy98@example.com\"}, {\"name\":\"Joe\", \"email\":\"joe@example.com\"}]**  | 
**params** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Pass the set of attributes to customize the template. For example, **{\"FNAME\":\"Joe\", \"LNAME\":\"Doe\"}**. It's **considered only if template is in New Template Language format**.  | [optional]
**bcc** | Option<[**Vec<models::SendSmtpEmailBccInner>**](sendSmtpEmail_bcc_inner.md)> | List of email addresses and names (_optional_) of the recipients in bcc  | [optional]
**cc** | Option<[**Vec<models::SendSmtpEmailCcInner>**](sendSmtpEmail_cc_inner.md)> | List of email addresses and names (_optional_) of the recipients in cc  | [optional]
**reply_to** | Option<[**models::SendSmtpEmailReplyTo**](sendSmtpEmail_replyTo.md)> |  | [optional]
**subject** | Option<**String**> | Custom subject specific to message version  | [optional]
**html_content** | Option<**String**> | HTML body of the message. **Mandatory if 'templateId' is not passed, ignored if 'templateId' is passed**  | [optional]
**text_content** | Option<**String**> | Plain Text body of the message. **Ignored if 'templateId' is passed**  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


