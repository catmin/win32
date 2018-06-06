---
Description: Enumerations that are used with authorization applications.
ms.assetid: e2f22838-102e-432c-9c82-06a3e0741374
title: Authorization Enumerations
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Authorization Enumerations

The following enumerations are used with authorization applications.

## In this section



| Topic                                                                                          | Description                                                                                                                                                                                                                                                                           |
|------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**ACCESS\_MODE**](https://www.bing.com/search?q=**ACCESS\_MODE**)<br/>                                                 | Contains values that indicate how the access rights in an [**EXPLICIT\_ACCESS**](/windows/desktop/api/AccCtrl/ns-accctrl-_explicit_access_a) structure apply to the trustee.<br/>                                                                                                                                      |
| [**ACL\_INFORMATION\_CLASS**](/windows/desktop/api/Winnt/ne-winnt-_acl_information_class)<br/>                            | Contains values that specify the type of information being assigned to or retrieved from an [access control list](https://msdn.microsoft.com/library/windows/desktop/ms721532#-security-access-control-list-gly) (ACL).<br/>                                                               |
| [**AUDIT\_EVENT\_TYPE**](/windows/desktop/api/Winnt/ne-winnt-_audit_event_type)<br/>                                      | Defines values that indicate the type of object being audited. The [**AccessCheckByTypeAndAuditAlarm**](/windows/desktop/api/Winbase/nf-winbase-accesscheckbytypeandauditalarma) and [**AccessCheckByTypeResultListAndAuditAlarm**](/windows/desktop/api/Winbase/nf-winbase-accesscheckbytyperesultlistandauditalarma) functions use these values.<br/>   |
| [**AUDIT\_PARAM\_TYPE**](/windows/desktop/api/Adtgen/ne-adtgen-_audit_param_type)<br/>                                      | Defines the type of audit parameters that are available.<br/>                                                                                                                                                                                                                   |
| [**AUTHZ\_CONTEXT\_INFORMATION\_CLASS**](/windows/desktop/api/Authz/ne-authz-_authz_context_information_class)<br/>       | Specifies the type of information to be retrieved from an existing AuthzClientContext. This enumeration is used by the [**AuthzGetInformationFromContext**](/windows/desktop/api/Authz/nf-authz-authzgetinformationfromcontext) function.<br/>                                                                  |
| [**AUTHZ\_SECURITY\_ATTRIBUTE\_OPERATION**](/windows/desktop/api/Authz/ne-authz-authz_security_attribute_operation)<br/> | Indicates the type of modification to be made to security attributes by a call to the [**AuthzModifySecurityAttributes**](/windows/desktop/api/Authz/nf-authz-authzmodifysecurityattributes) function.<br/>                                                                                                     |
| [**AUTHZ\_SID\_OPERATION**](/windows/desktop/api/Authz/ne-authz-authz_sid_operation)<br/>                                | Indicates the type of SID operations that can be made by a call to the [**AuthzModifySids**](/windows/desktop/api/Authz/nf-authz-authzmodifysids) function.<br/>                                                                                                                                                |
| [**AZ\_PROP\_CONSTANTS**](/windows/desktop/api/Azroles/ne-azroles-tagaz_prop_constants)<br/>                                    | Defines constants used by Authorization Manager.<br/>                                                                                                                                                                                                                           |
| [**MANDATORY\_LEVEL**](/windows/desktop/api/Winnt/ne-winnt-_mandatory_level)<br/>                                         | Lists the possible security levels.<br/>                                                                                                                                                                                                                                        |
| [**MULTIPLE\_TRUSTEE\_OPERATION**](/windows/desktop/api/AccCtrl/ne-accctrl-_multiple_trustee_operation)<br/>                  | Contains values that indicate whether a [**TRUSTEE**](/windows/desktop/api/AccCtrl/ns-accctrl-_trustee_a) structure is an impersonation trustee.<br/>                                                                                                                                                                  |
| [**PROG\_INVOKE\_SETTING**](/windows/desktop/api/AccCtrl/ne-accctrl-_progress_invoke_setting)<br/>                                | Indicates the initial setting of the function used to track the progress of a call to the [**TreeSetNamedSecurityInfo**](/windows/desktop/api/Aclapi/nf-aclapi-treesetnamedsecurityinfoa) or [**TreeResetNamedSecurityInfo**](/windows/desktop/api/Aclapi/nf-aclapi-treeresetnamedsecurityinfoa) function.<br/>                                       |
| [**SE\_OBJECT\_TYPE**](/windows/desktop/api/AccCtrl/ne-accctrl-_se_object_type)<br/>                                          | Contains values that correspond to the types of Windows objects that support security.<br/>                                                                                                                                                                                     |
| [**SECURITY\_IMPERSONATION\_LEVEL**](/windows/desktop/api/Winnt/ne-winnt-_security_impersonation_level)<br/>              | Contains values that specify security impersonation levels. Security impersonation levels govern the degree to which a server process can act on behalf of a client [process](https://msdn.microsoft.com/library/windows/desktop/ms721603#-security-process-gly).<br/>                                 |
| [**SI\_PAGE\_TYPE**](/windows/desktop/api/Aclui/ne-aclui-_si_page_type)<br/>                                              | Contains values that indicate the types of property pages in an access control editor property sheet.<br/>                                                                                                                                                                      |
| [**SID\_NAME\_USE**](/windows/desktop/api/Winnt/ne-winnt-_sid_name_use)<br/>                                              | Contains values that specify the type of a [security identifier](https://msdn.microsoft.com/library/windows/desktop/ms721625#-security-security-identifier-gly) (SID).<br/>                                                                                                                |
| [**TOKEN\_ELEVATION\_TYPE**](/windows/desktop/api/Winnt/ne-winnt-_token_elevation_type)<br/>                             | Indicates the elevation type of token being queried by the [**GetTokenInformation**](https://www.bing.com/search?q=**GetTokenInformation**) function or set by the [**SetTokenInformation**](https://www.bing.com/search?q=**SetTokenInformation**) function.<br/>                                                                          |
| [**TOKEN\_INFORMATION\_CLASS**](/windows/desktop/api/Winnt/ne-winnt-_token_information_class)<br/>                        | Contains values that specify the type of information being assigned to or retrieved from an [access token](https://msdn.microsoft.com/library/windows/desktop/ms721532#-security-access-token-gly).<br/>                                                                                          |
| [**TOKEN\_TYPE**](/windows/desktop/api/Winnt/ne-winnt-_token_type)<br/>                                                   | Contains values that differentiate between a [primary token](https://msdn.microsoft.com/library/windows/desktop/ms721603#-security-primary-token-gly) and an [impersonation token](https://msdn.microsoft.com/library/windows/desktop/ms721588#-security-impersonation-token-gly).<br/>                     |
| [**TRUSTEE\_FORM**](/windows/desktop/api/AccCtrl/ne-accctrl-_trustee_form)<br/>                                               | Values that indicate the type of data pointed to by the **ptstrName** member of the [**TRUSTEE**](/windows/desktop/api/AccCtrl/ns-accctrl-_trustee_a) structure.<br/>                                                                                                                                                  |
| [**TRUSTEE\_TYPE**](/windows/desktop/api/AccCtrl/ne-accctrl-_trustee_type)<br/>                                               | Values that indicate the type of trustee identified by a [**TRUSTEE**](/windows/desktop/api/AccCtrl/ns-accctrl-_trustee_a) structure.<br/>                                                                                                                                                                             |
| [**WELL\_KNOWN\_SID\_TYPE**](/windows/desktop/api/Winnt/ne-winnt-well_known_sid_type)<br/>                               | A list of commonly used [security identifiers](https://msdn.microsoft.com/library/windows/desktop/ms721625#-security-security-identifier-gly) (SIDs). Programs can pass these values to the [**CreateWellKnownSid**](https://www.bing.com/search?q=**CreateWellKnownSid**) function to create a SID from this list.<br/> |



 

 

 



