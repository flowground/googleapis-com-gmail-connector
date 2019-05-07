# ![LOGO](logo.png) Gmail **flow**ground Connector

## Description

A generated **flow**ground connector for the Gmail API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/gmail/v1/swagger.json<br/>
Generated at: 2019-05-07T17:41:42+03:00

## API Description

Access Gmail mailboxes including sending user email.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists the drafts in the user's mailbox.

*Tags:* `users`

#### Input Parameters
* `includeSpamTrash` - _optional_ - Include drafts from SPAM and TRASH in the results.
* `maxResults` - _optional_ - Maximum number of drafts to return.
* `pageToken` - _optional_ - Page token to retrieve a specific page of results in the list.
* `q` - _optional_ - Only return draft messages matching the specified query. Supports the same query format as the Gmail search box. For example, "from:someuser@example.com rfc822msgid: is:unread".
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a new draft with the DRAFT label.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Sends the specified, existing draft to the recipients in the To, Cc, and Bcc headers.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Immediately and permanently deletes the specified draft. Does not simply trash it.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the draft to delete.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the specified draft.

*Tags:* `users`

#### Input Parameters
* `format` - _optional_ - The format to return the draft in.
    Possible values: full, metadata, minimal, raw.
* `id` - _required_ - The ID of the draft to retrieve.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Replaces a draft's content.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the draft to update.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists the history of all changes to the given mailbox. History results are returned in chronological order (increasing historyId).

*Tags:* `users`

#### Input Parameters
* `historyTypes` - _optional_ - History types to be returned by the function
* `labelId` - _optional_ - Only return messages with a label matching the ID.
* `maxResults` - _optional_ - The maximum number of history records to return.
* `pageToken` - _optional_ - Page token to retrieve a specific page of results in the list.
* `startHistoryId` - _optional_ - Required. Returns history records after the specified startHistoryId. The supplied startHistoryId should be obtained from the historyId of a message, thread, or previous list response. History IDs increase chronologically but are not contiguous with random gaps in between valid IDs. Supplying an invalid or out of date startHistoryId typically returns an HTTP 404 error code. A historyId is typically valid for at least a week, but in some rare circumstances may be valid for only a few hours. If you receive an HTTP 404 error response, your application should perform a full sync. If you receive no nextPageToken in the response, there are no updates to retrieve and you can store the returned historyId for a future request.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists all labels in the user's mailbox.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a new label.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Immediately and permanently deletes the specified label and removes it from any messages and threads that it is applied to.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the label to delete.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the specified label.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the label to retrieve.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the specified label. This method supports patch semantics.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the label to update.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the specified label.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the label to update.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists the messages in the user's mailbox.

*Tags:* `users`

#### Input Parameters
* `includeSpamTrash` - _optional_ - Include messages from SPAM and TRASH in the results.
* `labelIds` - _optional_ - Only return messages with labels that match all of the specified label IDs.
* `maxResults` - _optional_ - Maximum number of messages to return.
* `pageToken` - _optional_ - Page token to retrieve a specific page of results in the list.
* `q` - _optional_ - Only return messages matching the specified query. Supports the same query format as the Gmail search box. For example, "from:someuser@example.com rfc822msgid:<somemsgid@example.com> is:unread". Parameter cannot be used when accessing the api using the gmail.metadata scope.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Directly inserts a message into only this user's mailbox similar to IMAP APPEND, bypassing most scanning and classification. Does not send a message.

*Tags:* `users`

#### Input Parameters
* `deleted` - _optional_ - Mark the email as permanently deleted (not TRASH) and only visible in Google Vault to a Vault administrator. Only used for G Suite accounts.
* `internalDateSource` - _optional_ - Source for Gmail's internal date of the message.
    Possible values: dateHeader, receivedTime.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes many messages by message ID. Provides no guarantees that messages were not already deleted or even existed at all.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Modifies the labels on the specified messages.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Imports a message into only this user's mailbox, with standard email delivery scanning and classification similar to receiving via SMTP. Does not send a message.

*Tags:* `users`

#### Input Parameters
* `deleted` - _optional_ - Mark the email as permanently deleted (not TRASH) and only visible in Google Vault to a Vault administrator. Only used for G Suite accounts.
* `internalDateSource` - _optional_ - Source for Gmail's internal date of the message.
    Possible values: dateHeader, receivedTime.
* `neverMarkSpam` - _optional_ - Ignore the Gmail spam classifier decision and never mark this email as SPAM in the mailbox.
* `processForCalendar` - _optional_ - Process calendar invites in the email and add any extracted meetings to the Google Calendar for this user.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Sends the specified message to the recipients in the To, Cc, and Bcc headers.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Immediately and permanently deletes the specified message. This operation cannot be undone. Prefer messages.trash instead.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the message to delete.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the specified message.

*Tags:* `users`

#### Input Parameters
* `format` - _optional_ - The format to return the message in.
    Possible values: full, metadata, minimal, raw.
* `id` - _required_ - The ID of the message to retrieve.
* `metadataHeaders` - _optional_ - When given and format is METADATA, only include headers specified.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Modifies the labels on the specified message.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the message to modify.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Moves the specified message to the trash.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the message to Trash.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Removes the specified message from the trash.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the message to remove from Trash.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the specified message attachment.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the attachment.
* `messageId` - _required_ - The ID of the message containing the attachment.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the current user's Gmail profile.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the auto-forwarding setting for the specified account.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates the auto-forwarding setting for the specified account. A verified forwarding address must be specified when auto-forwarding is enabled.<br/>
> <br/>
> This method is only available to service account clients that have been delegated domain-wide authority.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists the delegates for the specified account.<br/>
> <br/>
> This method is only available to service account clients that have been delegated domain-wide authority.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Adds a delegate with its verification status set directly to accepted, without sending any verification email. The delegate user must be a member of the same G Suite organization as the delegator user.<br/>
> <br/>
> Gmail imposes limtations on the number of delegates and delegators each user in a G Suite organization can have. These limits depend on your organization, but in general each user can have up to 25 delegates and up to 10 delegators.<br/>
> <br/>
> Note that a delegate user must be referred to by their primary email address, and not an email alias.<br/>
> <br/>
> Also note that when a new delegate is created, there may be up to a one minute delay before the new delegate is available for use.<br/>
> <br/>
> This method is only available to service account clients that have been delegated domain-wide authority.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Removes the specified delegate (which can be of any verification status), and revokes any verification that may have been required for using it.<br/>
> <br/>
> Note that a delegate user must be referred to by their primary email address, and not an email alias.<br/>
> <br/>
> This method is only available to service account clients that have been delegated domain-wide authority.

*Tags:* `users`

#### Input Parameters
* `delegateEmail` - _required_ - The email address of the user to be removed as a delegate.
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the specified delegate.<br/>
> <br/>
> Note that a delegate user must be referred to by their primary email address, and not an email alias.<br/>
> <br/>
> This method is only available to service account clients that have been delegated domain-wide authority.

*Tags:* `users`

#### Input Parameters
* `delegateEmail` - _required_ - The email address of the user whose delegate relationship is to be retrieved.
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists the message filters of a Gmail user.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a filter.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes a filter.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the filter to be deleted.
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets a filter.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the filter to be fetched.
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists the forwarding addresses for the specified account.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a forwarding address. If ownership verification is required, a message will be sent to the recipient and the resource's verification status will be set to pending; otherwise, the resource will be created with verification status set to accepted.<br/>
> <br/>
> This method is only available to service account clients that have been delegated domain-wide authority.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the specified forwarding address and revokes any verification that may have been required.<br/>
> <br/>
> This method is only available to service account clients that have been delegated domain-wide authority.

*Tags:* `users`

#### Input Parameters
* `forwardingEmail` - _required_ - The forwarding address to be deleted.
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the specified forwarding address.

*Tags:* `users`

#### Input Parameters
* `forwardingEmail` - _required_ - The forwarding address to be retrieved.
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets IMAP settings.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates IMAP settings.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets POP settings.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates POP settings.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists the send-as aliases for the specified account. The result includes the primary send-as address associated with the account as well as any custom "from" aliases.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Creates a custom "from" send-as alias. If an SMTP MSA is specified, Gmail will attempt to connect to the SMTP service to validate the configuration before creating the alias. If ownership verification is required for the alias, a message will be sent to the email address and the resource's verification status will be set to pending; otherwise, the resource will be created with verification status set to accepted. If a signature is provided, Gmail will sanitize the HTML before saving it with the alias.<br/>
> <br/>
> This method is only available to service account clients that have been delegated domain-wide authority.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the specified send-as alias. Revokes any verification that may have been required for using it.<br/>
> <br/>
> This method is only available to service account clients that have been delegated domain-wide authority.

*Tags:* `users`

#### Input Parameters
* `sendAsEmail` - _required_ - The send-as alias to be deleted.
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the specified send-as alias. Fails with an HTTP 404 error if the specified address is not a member of the collection.

*Tags:* `users`

#### Input Parameters
* `sendAsEmail` - _required_ - The send-as alias to be retrieved.
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates a send-as alias. If a signature is provided, Gmail will sanitize the HTML before saving it with the alias.<br/>
> <br/>
> Addresses other than the primary address for the account can only be updated by service account clients that have been delegated domain-wide authority. This method supports patch semantics.

*Tags:* `users`

#### Input Parameters
* `sendAsEmail` - _required_ - The send-as alias to be updated.
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates a send-as alias. If a signature is provided, Gmail will sanitize the HTML before saving it with the alias.<br/>
> <br/>
> Addresses other than the primary address for the account can only be updated by service account clients that have been delegated domain-wide authority.

*Tags:* `users`

#### Input Parameters
* `sendAsEmail` - _required_ - The send-as alias to be updated.
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists S/MIME configs for the specified send-as alias.

*Tags:* `users`

#### Input Parameters
* `sendAsEmail` - _required_ - The email address that appears in the "From:" header for mail sent using this alias.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Insert (upload) the given S/MIME config for the specified send-as alias. Note that pkcs12 format is required for the key.

*Tags:* `users`

#### Input Parameters
* `sendAsEmail` - _required_ - The email address that appears in the "From:" header for mail sent using this alias.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Deletes the specified S/MIME config for the specified send-as alias.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The immutable ID for the SmimeInfo.
* `sendAsEmail` - _required_ - The email address that appears in the "From:" header for mail sent using this alias.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the specified S/MIME config for the specified send-as alias.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The immutable ID for the SmimeInfo.
* `sendAsEmail` - _required_ - The email address that appears in the "From:" header for mail sent using this alias.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Sets the default S/MIME config for the specified send-as alias.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The immutable ID for the SmimeInfo.
* `sendAsEmail` - _required_ - The email address that appears in the "From:" header for mail sent using this alias.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Sends a verification email to the specified send-as alias address. The verification status must be pending.<br/>
> <br/>
> This method is only available to service account clients that have been delegated domain-wide authority.

*Tags:* `users`

#### Input Parameters
* `sendAsEmail` - _required_ - The send-as alias to be verified.
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets vacation responder settings.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Updates vacation responder settings.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - User's email address. The special value "me" can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Stop receiving push notifications for the given user mailbox.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Lists the threads in the user's mailbox.

*Tags:* `users`

#### Input Parameters
* `includeSpamTrash` - _optional_ - Include threads from SPAM and TRASH in the results.
* `labelIds` - _optional_ - Only return threads with labels that match all of the specified label IDs.
* `maxResults` - _optional_ - Maximum number of threads to return.
* `pageToken` - _optional_ - Page token to retrieve a specific page of results in the list.
* `q` - _optional_ - Only return threads matching the specified query. Supports the same query format as the Gmail search box. For example, "from:someuser@example.com rfc822msgid: is:unread". Parameter cannot be used when accessing the api using the gmail.metadata scope.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Immediately and permanently deletes the specified thread. This operation cannot be undone. Prefer threads.trash instead.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - ID of the Thread to delete.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Gets the specified thread.

*Tags:* `users`

#### Input Parameters
* `format` - _optional_ - The format to return the messages in.
    Possible values: full, metadata, minimal.
* `id` - _required_ - The ID of the thread to retrieve.
* `metadataHeaders` - _optional_ - When given and format is METADATA, only include headers specified.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Modifies the labels applied to the thread. This applies to all messages in the thread.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the thread to modify.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Moves the specified thread to the trash.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the thread to Trash.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Removes the specified thread from the trash.

*Tags:* `users`

#### Input Parameters
* `id` - _required_ - The ID of the thread to remove from Trash.
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Set up or update a push notification watch on the given user mailbox.

*Tags:* `users`

#### Input Parameters
* `userId` - _required_ - The user's email address. The special value me can be used to indicate the authenticated user.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

## License

**flow**ground :- Telekom iPaaS / googleapis-com-gmail-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
