---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Users API List assignments for user
  description: List assignments for user.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /audit/grade_change/assignments/{assignment_id}:
    get:
      summary: Query by assignment.
      description: Query by assignment..
      operationId: query-by-assignment
      x-api-path-slug: auditgrade-changeassignmentsassignment-id-get
      parameters:
      - in: query
        name: end_time
        description: The end of the time range from which you want events
      - in: query
        name: start_time
        description: The beginning of the time range from which you want events
      responses:
        200:
          description: OK
      tags:
      - Audit
      - Grade
      - Change
      - Assignments
      - Assignment
      - Id
  /courses/{course_id}/analytics/assignments:
    get:
      summary: Get course-level assignment data
      description: Get course-level assignment data.
      operationId: get-courselevel-assignment-data
      x-api-path-slug: coursescourse-idanalyticsassignments-get
      parameters:
      - in: query
        name: async
        description: If async is true, then the course_assignments call can happen
          asynch-nronously and MAY return a response containing a progress_url key
          instead ofnan assignments array
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Assignments
  /courses/{course_id}/analytics/users/student_id/assignments:
    get:
      summary: Get user-in-a-course-level assignment data
      description: Get user-in-a-course-level assignment data.
      operationId: get-userinacourselevel-assignment-data
      x-api-path-slug: coursescourse-idanalyticsusersstudent-idassignments-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Users
      - Student
      - Id
      - Assignments
  /courses/{course_id}/assignments:
    get:
      summary: List assignments
      description: List assignments.
      operationId: list-assignments
      x-api-path-slug: coursescourse-idassignments-get
      parameters:
      - in: query
        name: bucket
        description: If included, only return certain assignments depending on due
          date andnsubmission status
      - in: query
        name: include[]
        description: Associations to include with the assignment
      - in: query
        name: needs_grading_count_by_section
        description: Split up u201cneeds_grading_countu201d by sections into thenu201cneeds_grading_count_by_sectionu201d
          key, defaults to false
      - in: query
        name: override_assignment_dates
        description: Apply assignment overrides for each assignment, defaults to true
      - in: query
        name: search_term
        description: The partial title of the assignments to match and return
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
    post:
      summary: Create an assignment
      description: Create an assignment.
      operationId: create-an-assignment
      x-api-path-slug: coursescourse-idassignments-post
      parameters:
      - in: query
        name: assignment[allowed_extensions][]
        description: 'Allowed extensions if submission_types includes u201conline_uploadu201dnnExample:nnallowed_extensions:
          [&quot;docx&quot;,&quot;ppt&quot;]'
      - in: query
        name: assignment[assignment_group_id]
        description: The assignment group id to put the assignment in
      - in: query
        name: assignment[assignment_overrides][]
        description: List of overrides for the assignment
      - in: query
        name: assignment[automatic_peer_reviews]
        description: Whether peer reviews will be assigned automatically by Canvas
          or ifnteachers must manually assign peer reviews
      - in: query
        name: assignment[description]
        description: The assignment&#39;s description, supports HTML
      - in: query
        name: assignment[due_at]
        description: The day/time the assignment is due
      - in: query
        name: assignment[external_tool_tag_attributes]
        description: 'Hash of attributes if submission_types is [u201cexternal_toolu201d]
          Example:nnexternal_tool_tag_attributes: {n  %r/ url to the external tooln  url:
          &quot;http://instructure'
      - in: query
        name: assignment[grade_group_students_individually]
        description: If this is a group assignment, teachers have the options to grade
          studentsnindividually
      - in: query
        name: assignment[grading_standard_id]
        description: The grading standard id to set for the course
      - in: query
        name: assignment[grading_type]
        description: The strategy used for grading the assignment
      - in: query
        name: assignment[group_category_id]
        description: If present, the assignment will become a group assignment assigned
          to thengroup
      - in: query
        name: assignment[integration_data]
        description: Data related to third party integrations, JSON string required
      - in: query
        name: assignment[integration_id]
        description: Unique ID from third party integrations
      - in: query
        name: assignment[lock_at]
        description: The day/time the assignment is locked after
      - in: query
        name: assignment[muted]
        description: Whether this assignment is muted
      - in: query
        name: assignment[name]
        description: The assignment name
      - in: query
        name: assignment[notify_of_update]
        description: If true, Canvas will send a notification to students in the class
          notifyingnthem that the content has changed
      - in: query
        name: assignment[only_visible_to_overrides]
        description: Whether this assignment is only visible to overrides (Only useful
          ifn&#39;differentiated assignments&#39; account setting is on)
      - in: query
        name: assignment[peer_reviews]
        description: If submission_types does not include external_tool,discussion_topic,nonline_quiz,
          or on_paper, determines whether or not peer reviews will benturned on for
          the assignment
      - in: query
        name: assignment[points_possible]
        description: The maximum points possible on the assignment
      - in: query
        name: assignment[position]
        description: The position of this assignment in the group when displaying
          assignmentnlists
      - in: query
        name: assignment[published]
        description: Whether this assignment is published
      - in: query
        name: assignment[submission_types][]
        description: List of supported submission types for the assignment
      - in: query
        name: assignment[turnitin_enabled]
        description: Only applies when the Turnitin plugin is enabled for a course
          and thensubmission_types array includes u201conline_uploadu201d
      - in: query
        name: assignment[turnitin_settings]
        description: Settings to send along to turnitin
      - in: query
        name: assignment[unlock_at]
        description: The day/time the assignment is unlocked
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
  /courses/{course_id}/assignments/assignment_id/gradeable_students:
    get:
      summary: List gradeable students
      description: List gradeable students.
      operationId: list-gradeable-students
      x-api-path-slug: coursescourse-idassignmentsassignment-idgradeable-students-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Gradeable
      - Students
  /courses/{course_id}/assignments/assignment_id/moderated_students:
    get:
      summary: List students selected for moderation
      description: List students selected for moderation.
      operationId: list-students-selected-for-moderation
      x-api-path-slug: coursescourse-idassignmentsassignment-idmoderated-students-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Moderated
      - Students
    post:
      summary: Select students for moderation
      description: Select students for moderation.
      operationId: select-students-for-moderation
      x-api-path-slug: coursescourse-idassignmentsassignment-idmoderated-students-post
      parameters:
      - in: query
        name: student_ids[]
        description: user ids for students to select for moderation
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Moderated
      - Students
  /courses/{course_id}/assignments/assignment_id/overrides:
    get:
      summary: List assignment overrides
      description: List assignment overrides.
      operationId: list-assignment-overrides
      x-api-path-slug: coursescourse-idassignmentsassignment-idoverrides-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Overrides
    post:
      summary: Create an assignment override
      description: Create an assignment override.
      operationId: create-an-assignment-override
      x-api-path-slug: coursescourse-idassignmentsassignment-idoverrides-post
      parameters:
      - in: query
        name: assignment_override[course_section_id]
        description: The ID of the override&#39;s target section
      - in: query
        name: assignment_override[due_at]
        description: The day/time the overridden assignment is due
      - in: query
        name: assignment_override[group_id]
        description: The ID of the override&#39;s target group
      - in: query
        name: assignment_override[lock_at]
        description: The day/time the overridden assignment becomes locked
      - in: query
        name: assignment_override[student_ids][]
        description: The IDs of the override&#39;s target students
      - in: query
        name: assignment_override[title]
        description: The title of the adhoc assignment override
      - in: query
        name: assignment_override[unlock_at]
        description: The day/time the overridden assignment becomes unlocked
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Overrides
  /courses/{course_id}/assignments/assignment_id/overrides/{id}:
    delete:
      summary: Delete an assignment override
      description: Delete an assignment override.
      operationId: delete-an-assignment-override
      x-api-path-slug: coursescourse-idassignmentsassignment-idoverridesid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Overrides
      - Id
    get:
      summary: Get a single assignment override
      description: Get a single assignment override.
      operationId: get-a-single-assignment-override
      x-api-path-slug: coursescourse-idassignmentsassignment-idoverridesid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Overrides
      - Id
    put:
      summary: Update an assignment override
      description: Update an assignment override.
      operationId: update-an-assignment-override
      x-api-path-slug: coursescourse-idassignmentsassignment-idoverridesid-put
      parameters:
      - in: query
        name: assignment_override[due_at]
        description: The day/time the overridden assignment is due
      - in: query
        name: assignment_override[lock_at]
        description: The day/time the overridden assignment becomes locked
      - in: query
        name: assignment_override[student_ids][]
        description: The IDs of the override&#39;s target students
      - in: query
        name: assignment_override[title]
        description: The title of an adhoc assignment override
      - in: query
        name: assignment_override[unlock_at]
        description: The day/time the overridden assignment becomes unlocked
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Overrides
      - Id
  /courses/{course_id}/assignments/assignment_id/peer_reviews:
    get:
      summary: Get all Peer Reviews
      description: Get all peer reviews.
      operationId: get-all-peer-reviews
      x-api-path-slug: coursescourse-idassignmentsassignment-idpeer-reviews-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the peer review
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Peer
      - Reviews
  /courses/{course_id}/assignments/assignment_id/provisional_grades/publish:
    post:
      summary: Publish provisional grades for an assignment
      description: Publish provisional grades for an assignment.
      operationId: publish-provisional-grades-for-an-assignment
      x-api-path-slug: coursescourse-idassignmentsassignment-idprovisional-gradespublish-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Provisional
      - Grades
      - Publish
  /courses/{course_id}/assignments/assignment_id/provisional_grades/status:
    get:
      summary: Show provisional grade status for a student
      description: Show provisional grade status for a student.
      operationId: show-provisional-grade-status-for-a-student
      x-api-path-slug: coursescourse-idassignmentsassignment-idprovisional-gradesstatus-get
      parameters:
      - in: query
        name: student_id
        description: The id of the student to show the status for
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Provisional
      - Grades
      - Status
  /courses/{course_id}/assignments/assignment_id/provisional_grades/{provisional_grade_id}/copy_to_final_mark:
    post:
      summary: Copy provisional grade
      description: Copy provisional grade.
      operationId: copy-provisional-grade
      x-api-path-slug: coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idcopy-to-final-mark-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Provisional
      - Grades
      - Provisional
      - Grade
      - Id
      - Copy
      - To
      - Final
      - Mark
  /courses/{course_id}/assignments/assignment_id/provisional_grades/{provisional_grade_id}/select:
    put:
      summary: Select provisional grade
      description: Select provisional grade.
      operationId: select-provisional-grade
      x-api-path-slug: coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idselect-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Provisional
      - Grades
      - Provisional
      - Grade
      - Id
      - Select
  /courses/{course_id}/assignments/assignment_id/submissions:
    get:
      summary: List assignment submissions
      description: List assignment submissions.
      operationId: list-assignment-submissions
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissions-get
      parameters:
      - in: query
        name: grouped
        description: If this argument is true, the response will be grouped by student
          groups
      - in: query
        name: include[]
        description: Associations to include with the group
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
    post:
      summary: Submit an assignment
      description: Submit an assignment.
      operationId: submit-an-assignment
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissions-post
      parameters:
      - in: query
        name: comment[text_comment]
        description: Include a textual comment with the submission
      - in: query
        name: submission[body]
        description: Submit the assignment as an HTML document snippet
      - in: query
        name: submission[file_ids][]
        description: Submit the assignment as a set of one or more previously uploaded
          filesnresiding in the submitting user&#39;s files section (or the group&#39;snfiles
          section, for group assignments)
      - in: query
        name: submission[media_comment_id]
        description: The media comment id to submit
      - in: query
        name: submission[media_comment_type]
        description: The type of media comment being submitted
      - in: query
        name: submission[submission_type]
        description: The type of submission being made
      - in: query
        name: submission[url]
        description: Submit the assignment as a URL
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
  /courses/{course_id}/assignments/assignment_id/submissions/update_grades:
    post:
      summary: Grade or comment on multiple submissions
      description: Grade or comment on multiple submissions.
      operationId: grade-or-comment-on-multiple-submissions
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsupdate-grades-post
      parameters:
      - in: query
        name: grade_data[student_id][file_ids][]
        description: See documentation for the comment[] arguments in thenSubmissions
          Update documentation
      - in: query
        name: grade_data[student_id][group_comment]
        description: no description
      - in: query
        name: grade_data[student_id][media_comment_id]
        description: no description
      - in: query
        name: grade_data[student_id][media_comment_type]
        description: 'no descriptionnn        n        n          Allowed values:
          audio, video'
      - in: query
        name: grade_data[student_id][posted_grade]
        description: See documentation for the posted_grade argument in thenSubmissions
          Update documentation
      - in: query
        name: grade_data[student_id][rubric_assessment]
        description: See documentation for the rubric_assessment argument in thenSubmissions
          Update documentation
      - in: query
        name: grade_data[student_id][text_comment]
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - Update
      - Grades
  /courses/{course_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews:
    delete:
      summary: Create Peer Review
      description: Create peer review.
      operationId: create-peer-review
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete
      parameters:
      - in: query
        name: user_id
        description: user_id to delete as reviewer on this assignment
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - Submission
      - Id
      - Peer
      - Reviews
    get:
      summary: Get all Peer Reviews
      description: Get all peer reviews.
      operationId: get-all-peer-reviews
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the peer review
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - Submission
      - Id
      - Peer
      - Reviews
    post:
      summary: Create Peer Review
      description: Create peer review.
      operationId: create-peer-review
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post
      parameters:
      - in: query
        name: user_id
        description: user_id to assign as reviewer on this assignment
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - Submission
      - Id
      - Peer
      - Reviews
  /courses/{course_id}/assignments/assignment_id/submissions/{user_id}:
    get:
      summary: Get a single submission
      description: Get a single submission.
      operationId: get-a-single-submission
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-id-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the group
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
    put:
      summary: Grade or comment on a submission
      description: Grade or comment on a submission.
      operationId: grade-or-comment-on-a-submission
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-id-put
      parameters:
      - in: query
        name: comment[file_ids][]
        description: Attach files to this comment that were previously uploaded using
          thenSubmission Comment API&#39;s files action
      - in: query
        name: comment[group_comment]
        description: Whether or not this comment should be sent to the entire group
          (defaults tonfalse)
      - in: query
        name: comment[media_comment_id]
        description: Add an audio/video comment to the submission
      - in: query
        name: comment[media_comment_type]
        description: The type of media comment being added
      - in: query
        name: comment[text_comment]
        description: Add a textual comment to the submission
      - in: query
        name: include[visibility]
        description: Whether this assignment is visible to the owner of the submission
      - in: query
        name: rubric_assessment
        description: Assign a rubric assessment to this assignment submission
      - in: query
        name: submission[excuse]
        description: Sets the u201cexcusedu201d status of an assignment
      - in: query
        name: submission[posted_grade]
        description: Assign a score to the submission, updating both the u201cscoreu201d
          and u201cgradeu201dnfields on the submission record
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
  /courses/{course_id}/assignments/assignment_id/submissions/{user_id}/comments/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-idcommentsfiles-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Comments
      - Files
  /courses/{course_id}/assignments/assignment_id/submissions/{user_id}/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Files
  /courses/{course_id}/assignments/assignment_id/submissions/{user_id}/read:
    delete:
      summary: Mark submission as unread
      description: Mark submission as unread.
      operationId: mark-submission-as-unread
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-idread-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Read
    put:
      summary: Mark submission as read
      description: Mark submission as read.
      operationId: mark-submission-as-read
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-idread-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Read
  /courses/{course_id}/assignments/id:
    delete:
      summary: Delete an assignment
      description: Delete an assignment.
      operationId: delete-an-assignment
      x-api-path-slug: coursescourse-idassignmentsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Id
    get:
      summary: Get a single assignment
      description: Get a single assignment.
      operationId: get-a-single-assignment
      x-api-path-slug: coursescourse-idassignmentsid-get
      parameters:
      - in: query
        name: all_dates
        description: All dates associated with the assignment, if applicable
      - in: query
        name: include[]
        description: Associations to include with the assignment
      - in: query
        name: needs_grading_count_by_section
        description: Split up u201cneeds_grading_countu201d by sections into thenu201cneeds_grading_count_by_sectionu201d
          key, defaults to false
      - in: query
        name: override_assignment_dates
        description: Apply assignment overrides to the assignment, defaults to true
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Id
    put:
      summary: Edit an assignment
      description: Edit an assignment.
      operationId: edit-an-assignment
      x-api-path-slug: coursescourse-idassignmentsid-put
      parameters:
      - in: query
        name: assignment[allowed_extensions][]
        description: 'Allowed extensions if submission_types includes u201conline_uploadu201dnnExample:nnallowed_extensions:
          [&quot;docx&quot;,&quot;ppt&quot;]'
      - in: query
        name: assignment[assignment_group_id]
        description: The assignment group id to put the assignment in
      - in: query
        name: assignment[assignment_overrides][]
        description: List of overrides for the assignment
      - in: query
        name: assignment[automatic_peer_reviews]
        description: Whether peer reviews will be assigned automatically by Canvas
          or ifnteachers must manually assign peer reviews
      - in: query
        name: assignment[description]
        description: The assignment&#39;s description, supports HTML
      - in: query
        name: assignment[due_at]
        description: The day/time the assignment is due
      - in: query
        name: assignment[external_tool_tag_attributes]
        description: 'Hash of attributes if submission_types is [u201cexternal_toolu201d]
          Example:nnexternal_tool_tag_attributes: {n  %r/ url to the external tooln  url:
          &quot;http://instructure'
      - in: query
        name: assignment[grade_group_students_individually]
        description: If this is a group assignment, teachers have the options to grade
          studentsnindividually
      - in: query
        name: assignment[grading_standard_id]
        description: The grading standard id to set for the course
      - in: query
        name: assignment[grading_type]
        description: The strategy used for grading the assignment
      - in: query
        name: assignment[group_category_id]
        description: If present, the assignment will become a group assignment assigned
          to thengroup
      - in: query
        name: assignment[integration_data]
        description: Data related to third party integrations, JSON string required
      - in: query
        name: assignment[integration_id]
        description: Unique ID from third party integrations
      - in: query
        name: assignment[lock_at]
        description: The day/time the assignment is locked after
      - in: query
        name: assignment[muted]
        description: Whether this assignment is muted
      - in: query
        name: assignment[name]
        description: The assignment name
      - in: query
        name: assignment[notify_of_update]
        description: If true, Canvas will send a notification to students in the class
          notifyingnthem that the content has changed
      - in: query
        name: assignment[only_visible_to_overrides]
        description: Whether this assignment is only visible to overrides (Only useful
          ifn&#39;differentiated assignments&#39; account setting is on)
      - in: query
        name: assignment[peer_reviews]
        description: If submission_types does not include external_tool,discussion_topic,nonline_quiz,
          or on_paper, determines whether or not peer reviews will benturned on for
          the assignment
      - in: query
        name: assignment[points_possible]
        description: The maximum points possible on the assignment
      - in: query
        name: assignment[position]
        description: The position of this assignment in the group when displaying
          assignmentnlists
      - in: query
        name: assignment[published]
        description: Whether this assignment is published
      - in: query
        name: assignment[submission_types][]
        description: List of supported submission types for the assignment
      - in: query
        name: assignment[turnitin_enabled]
        description: Only applies when the Turnitin plugin is enabled for a course
          and thensubmission_types array includes u201conline_uploadu201d
      - in: query
        name: assignment[turnitin_settings]
        description: Settings to send along to turnitin
      - in: query
        name: assignment[unlock_at]
        description: The day/time the assignment is unlocked
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Id
  /courses/{course_id}/gradebook_history/date/graders/{grader_id}/assignments/assignment_id/submissions:
    get:
      summary: Lists submissions
      description: Lists submissions.
      operationId: lists-submissions
      x-api-path-slug: coursescourse-idgradebook-historydategradersgrader-idassignmentsassignment-idsubmissions-get
      parameters:
      - in: query
        name: assignment_id
        description: The ID of the assignment for which you want to see submissions
      - in: query
        name: course_id
        description: The id of the contextual course for this API call
      - in: query
        name: date
        description: The date for which you would like to see submissions
      - in: query
        name: grader_id
        description: The ID of the grader for which you want to see submissions
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Gradebook
      - History
      - Date
      - Graders
      - Grader
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
  /courses/{course_id}/assignment_groups:
    get:
      summary: List assignment groups
      description: List assignment groups.
      operationId: list-assignment-groups
      x-api-path-slug: coursescourse-idassignment-groups-get
      parameters:
      - in: query
        name: grading_period_id
        description: The id of the grading period in which assignment groups are being
          requestedn(Requires the Multiple Grading Periods feature turned on
      - in: query
        name: include[]
        description: Associations to include with the group
      - in: query
        name: override_assignment_dates
        description: Apply assignment overrides for each assignment, defaults to true
      - in: query
        name: scope_assignments_to_student
        description: If true, all assignments returned will apply to the current user
          in thenspecified grading period
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
    post:
      summary: Create an Assignment Group
      description: Create an assignment group.
      operationId: create-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groups-post
      parameters:
      - in: query
        name: group_weight
        description: The percent of the total grade that this assignment group represents
      - in: query
        name: name
        description: The assignment group&#39;s name
      - in: query
        name: position
        description: The position of this assignment group in relation to the other
          assignmentngroups
      - in: query
        name: rules
        description: The grading rules that are applied within this assignment group
          See thenAssignment Group object definition for format
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
  /courses/{course_id}/assignment_groups/assignment_group_id:
    delete:
      summary: Destroy an Assignment Group
      description: Destroy an assignment group.
      operationId: destroy-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groupsassignment-group-id-delete
      parameters:
      - in: query
        name: move_assignments_to
        description: The ID of an active Assignment Group to which the assignments
          that arencurrently assigned to the destroyed Assignment Group will be assigned
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
      - Assignment
      - Group
      - Id
    get:
      summary: Get an Assignment Group
      description: Get an assignment group.
      operationId: get-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groupsassignment-group-id-get
      parameters:
      - in: query
        name: grading_period_id
        description: The id of the grading period in which assignment groups are being
          requestedn(Requires the Multiple Grading Periods account feature turned
          on)
      - in: query
        name: include[]
        description: Associations to include with the group
      - in: query
        name: override_assignment_dates
        description: Apply assignment overrides for each assignment, defaults to true
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
      - Assignment
      - Group
      - Id
    put:
      summary: Edit an Assignment Group
      description: Edit an assignment group.
      operationId: edit-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groupsassignment-group-id-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
      - Assignment
      - Group
      - Id
  /courses/{course_id}/quizzes/assignment_overrides:
    get:
      summary: Retrieve assignment-overridden dates for quizzes
      description: Retrieve assignment-overridden dates for quizzes.
      operationId: retrieve-assignmentoverridden-dates-for-quizzes
      x-api-path-slug: coursescourse-idquizzesassignment-overrides-get
      parameters:
      - in: query
        name: quiz_assignment_overrides[0][quiz_ids][]
        description: An array of quiz IDs
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Assignment
      - Overrides
  /groups/{group_id}/assignments/assignment_id/override:
    get:
      summary: Redirect to the assignment override for a group
      description: Redirect to the assignment override for a group.
      operationId: redirect-to-the-assignment-override-for-a-group
      x-api-path-slug: groupsgroup-idassignmentsassignment-idoverride-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Assignments
      - Assignment
      - Id
      - Override
  /sections/{course_section_id}/assignments/assignment_id/override:
    get:
      summary: Redirect to the assignment override for a section
      description: Redirect to the assignment override for a section.
      operationId: redirect-to-the-assignment-override-for-a-section
      x-api-path-slug: sectionscourse-section-idassignmentsassignment-idoverride-get
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Course
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Override
  /sections/{section_id}/assignments/assignment_id/peer_reviews:
    get:
      summary: Get all Peer Reviews
      description: Get all peer reviews.
      operationId: get-all-peer-reviews
      x-api-path-slug: sectionssection-idassignmentsassignment-idpeer-reviews-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the peer review
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Peer
      - Reviews
  /sections/{section_id}/assignments/assignment_id/submissions:
    get:
      summary: List assignment submissions
      description: List assignment submissions.
      operationId: list-assignment-submissions
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissions-get
      parameters:
      - in: query
        name: grouped
        description: If this argument is true, the response will be grouped by student
          groups
      - in: query
        name: include[]
        description: Associations to include with the group
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
    post:
      summary: Submit an assignment
      description: Submit an assignment.
      operationId: submit-an-assignment
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissions-post
      parameters:
      - in: query
        name: comment[text_comment]
        description: Include a textual comment with the submission
      - in: query
        name: submission[body]
        description: Submit the assignment as an HTML document snippet
      - in: query
        name: submission[file_ids][]
        description: Submit the assignment as a set of one or more previously uploaded
          filesnresiding in the submitting user&#39;s files section (or the group&#39;snfiles
          section, for group assignments)
      - in: query
        name: submission[media_comment_id]
        description: The media comment id to submit
      - in: query
        name: submission[media_comment_type]
        description: The type of media comment being submitted
      - in: query
        name: submission[submission_type]
        description: The type of submission being made
      - in: query
        name: submission[url]
        description: Submit the assignment as a URL
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
  /sections/{section_id}/assignments/assignment_id/submissions/update_grades:
    post:
      summary: Grade or comment on multiple submissions
      description: Grade or comment on multiple submissions.
      operationId: grade-or-comment-on-multiple-submissions
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsupdate-grades-post
      parameters:
      - in: query
        name: grade_data[student_id][file_ids][]
        description: See documentation for the comment[] arguments in thenSubmissions
          Update documentation
      - in: query
        name: grade_data[student_id][group_comment]
        description: no description
      - in: query
        name: grade_data[student_id][media_comment_id]
        description: no description
      - in: query
        name: grade_data[student_id][media_comment_type]
        description: 'no descriptionnn        n        n          Allowed values:
          audio, video'
      - in: query
        name: grade_data[student_id][posted_grade]
        description: See documentation for the posted_grade argument in thenSubmissions
          Update documentation
      - in: query
        name: grade_data[student_id][rubric_assessment]
        description: See documentation for the rubric_assessment argument in thenSubmissions
          Update documentation
      - in: query
        name: grade_data[student_id][text_comment]
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - Update
      - Grades
  /sections/{section_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews:
    delete:
      summary: Create Peer Review
      description: Create peer review.
      operationId: create-peer-review
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete
      parameters:
      - in: query
        name: user_id
        description: user_id to delete as reviewer on this assignment
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - Submission
      - Id
      - Peer
      - Reviews
    get:
      summary: Get all Peer Reviews
      description: Get all peer reviews.
      operationId: get-all-peer-reviews
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the peer review
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - Submission
      - Id
      - Peer
      - Reviews
    post:
      summary: Create Peer Review
      description: Create peer review.
      operationId: create-peer-review
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post
      parameters:
      - in: query
        name: user_id
        description: user_id to assign as reviewer on this assignment
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - Submission
      - Id
      - Peer
      - Reviews
  /sections/{section_id}/assignments/assignment_id/submissions/{user_id}:
    get:
      summary: Get a single submission
      description: Get a single submission.
      operationId: get-a-single-submission
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsuser-id-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the group
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
    put:
      summary: Grade or comment on a submission
      description: Grade or comment on a submission.
      operationId: grade-or-comment-on-a-submission
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsuser-id-put
      parameters:
      - in: query
        name: comment[file_ids][]
        description: Attach files to this comment that were previously uploaded using
          thenSubmission Comment API&#39;s files action
      - in: query
        name: comment[group_comment]
        description: Whether or not this comment should be sent to the entire group
          (defaults tonfalse)
      - in: query
        name: comment[media_comment_id]
        description: Add an audio/video comment to the submission
      - in: query
        name: comment[media_comment_type]
        description: The type of media comment being added
      - in: query
        name: comment[text_comment]
        description: Add a textual comment to the submission
      - in: query
        name: include[visibility]
        description: Whether this assignment is visible to the owner of the submission
      - in: query
        name: rubric_assessment
        description: Assign a rubric assessment to this assignment submission
      - in: query
        name: submission[excuse]
        description: Sets the u201cexcusedu201d status of an assignment
      - in: query
        name: submission[posted_grade]
        description: Assign a score to the submission, updating both the u201cscoreu201d
          and u201cgradeu201dnfields on the submission record
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
  /sections/{section_id}/assignments/assignment_id/submissions/{user_id}/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsuser-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Files
  /sections/{section_id}/assignments/assignment_id/submissions/{user_id}/read:
    delete:
      summary: Mark submission as unread
      description: Mark submission as unread.
      operationId: mark-submission-as-unread
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsuser-idread-delete
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Read
    put:
      summary: Mark submission as read
      description: Mark submission as read.
      operationId: mark-submission-as-read
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsuser-idread-put
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Read
  /users/{user_id}/courses/course_id/assignments:
    get:
      summary: List assignments for user
      description: List assignments for user.
      operationId: list-assignments-for-user
      x-api-path-slug: usersuser-idcoursescourse-idassignments-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Courses
      - Course
      - Id
      - Assignments
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