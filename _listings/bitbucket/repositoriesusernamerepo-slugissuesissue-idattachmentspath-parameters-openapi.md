---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Repositories Username Repo Slug Issues Issue  Attachments
    Path
  description: Parameters repositories username repo slug issues issue  attachments
    path
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}/issues/{issue_id}/attachments:
    get:
      summary: Get Repositories Username Repo Slug Issues Issue  Attachments
      description: |-
        Returns all attachments for this issue.

        This returns the files' meta data. This does not return the files'
        actual contents.

        The files are always ordered by their upload date.
      operationId: getRepositoriesUsernameRepoSlugIssuesIssueAttachments
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idattachments-get
      parameters:
      - in: path
        name: issue_id
        description: The issues id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Attachments
    parameters:
      summary: Parameters Repositories Username Repo Slug Issues Issue  Attachments
      description: Parameters repositories username repo slug issues issue  attachments
      operationId: parametersRepositoriesUsernameRepoSlugIssuesIssueAttachments
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idattachments-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Attachments
    post:
      summary: Add Repositories Username Repo Slug Issues Issue  Attachments
      description: |-
        Upload new issue attachments.

        To upload files, perform a `multipart/form-data` POST containing one
        or more file fields.

        When a file is uploaded with the same name as an existing attachment,
        then the existing file will be replaced.
      operationId: postRepositoriesUsernameRepoSlugIssuesIssueAttachments
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idattachments-post
      parameters:
      - in: path
        name: issue_id
        description: The issues id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Attachments
  /repositories/{username}/{repo_slug}/issues/{issue_id}/attachments/{path}:
    delete:
      summary: Delete Repositories Username Repo Slug Issues Issue  Attachments Path
      description: Delete repositories username repo slug issues issue  attachments
        path
      operationId: deleteRepositoriesUsernameRepoSlugIssuesIssueAttachmentsPath
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idattachmentspath-delete
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Attachments
      - Path
    get:
      summary: Get Repositories Username Repo Slug Issues Issue  Attachments Path
      description: |-
        Returns the contents of the specified file attachment.

        Note that this endpoint does not return a JSON response, but instead
        returns a redirect pointing to the actual file that in turn will return
        the raw contents.

        The redirect URL contains a one-time token that has a limited lifetime.
        As a result, the link should not be persisted, stored, or shared.
      operationId: getRepositoriesUsernameRepoSlugIssuesIssueAttachmentsPath
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idattachmentspath-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Attachments
      - Path
    parameters:
      summary: Parameters Repositories Username Repo Slug Issues Issue  Attachments
        Path
      description: Parameters repositories username repo slug issues issue  attachments
        path
      operationId: parametersRepositoriesUsernameRepoSlugIssuesIssueAttachmentsPath
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idattachmentspath-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Attachments
      - Path
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---