---
name: Instructure
x-slug: instructure
description: Instructure makes software that makes smarter people. Products include
  Canvas LMS, Bridge and Canvas Network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
x-kinRank: "8"
x-alexaRank: "367"
tags: Assignments
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/apis.md
specificationVersion: "0.14"
apis:
- name: Instructure Canvas Audit API Query by assignment.
  x-api-slug: instructure-canvas-audit-api
  description: Query by assignment..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//audit/grade_change/assignments/{assignment_id}
  tags: Audit,Grade,Change,Assignments,Assignment,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/auditgrade-changeassignmentsassignment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/auditgrade-changeassignmentsassignment-id-get-openapi.md
- name: Instructure Canvas Audit API
  x-api-slug: instructure-canvas-audit-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/openapi.md
- name: Instructure Canvas Courses API Get course-level assignment data
  x-api-slug: instructure-canvas-courses-api
  description: Get course-level assignment data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/analytics/assignments
  tags: Courses,Course,Id,Analytics,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idanalyticsassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idanalyticsassignments-get-openapi.md
- name: Instructure Canvas Courses API Get user-in-a-course-level assignment data
  x-api-slug: instructure-canvas-courses-api
  description: Get user-in-a-course-level assignment data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/analytics/users/student_id/assignments
  tags: Courses,Course,Id,Analytics,Users,Student,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idassignments-get-openapi.md
- name: Instructure Canvas Courses API List assignments
  x-api-slug: instructure-canvas-courses-api
  description: List assignments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments
  tags: Courses,Course,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignments-get-openapi.md
- name: Instructure Canvas Courses API Create an assignment
  x-api-slug: instructure-canvas-courses-api
  description: Create an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments
  tags: Courses,Course,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignments-post-openapi.md
- name: Instructure Canvas Courses API List gradeable students
  x-api-slug: instructure-canvas-courses-api
  description: List gradeable students.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/gradeable_students
  tags: Courses,Course,Id,Assignments,Assignment,Id,Gradeable,Students
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idgradeable-students-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idgradeable-students-get-openapi.md
- name: Instructure Canvas Courses API List students selected for moderation
  x-api-slug: instructure-canvas-courses-api
  description: List students selected for moderation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/moderated_students
  tags: Courses,Course,Id,Assignments,Assignment,Id,Moderated,Students
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idmoderated-students-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idmoderated-students-get-openapi.md
- name: Instructure Canvas Courses API Select students for moderation
  x-api-slug: instructure-canvas-courses-api
  description: Select students for moderation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/moderated_students
  tags: Courses,Course,Id,Assignments,Assignment,Id,Moderated,Students
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idmoderated-students-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idmoderated-students-post-openapi.md
- name: Instructure Canvas Courses API List assignment overrides
  x-api-slug: instructure-canvas-courses-api
  description: List assignment overrides.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/overrides
  tags: Courses,Course,Id,Assignments,Assignment,Id,Overrides
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverrides-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverrides-get-openapi.md
- name: Instructure Canvas Courses API Create an assignment override
  x-api-slug: instructure-canvas-courses-api
  description: Create an assignment override.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/overrides
  tags: Courses,Course,Id,Assignments,Assignment,Id,Overrides
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverrides-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverrides-post-openapi.md
- name: Instructure Canvas Courses API Delete an assignment override
  x-api-slug: instructure-canvas-courses-api
  description: Delete an assignment override.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/overrides/{id}
  tags: Courses,Course,Id,Assignments,Assignment,Id,Overrides,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-delete-openapi.md
- name: Instructure Canvas Courses API Get a single assignment override
  x-api-slug: instructure-canvas-courses-api
  description: Get a single assignment override.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/overrides/{id}
  tags: Courses,Course,Id,Assignments,Assignment,Id,Overrides,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-get-openapi.md
- name: Instructure Canvas Courses API Update an assignment override
  x-api-slug: instructure-canvas-courses-api
  description: Update an assignment override.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/overrides/{id}
  tags: Courses,Course,Id,Assignments,Assignment,Id,Overrides,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-put-openapi.md
- name: Instructure Canvas Courses API Get all Peer Reviews
  x-api-slug: instructure-canvas-courses-api
  description: Get all peer reviews.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/peer_reviews
  tags: Courses,Course,Id,Assignments,Assignment,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idpeer-reviews-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idpeer-reviews-get-openapi.md
- name: Instructure Canvas Courses API Publish provisional grades for an assignment
  x-api-slug: instructure-canvas-courses-api
  description: Publish provisional grades for an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/provisional_grades/publish
  tags: Courses,Course,Id,Assignments,Assignment,Id,Provisional,Grades,Publish
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradespublish-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradespublish-post-openapi.md
- name: Instructure Canvas Courses API Show provisional grade status for a student
  x-api-slug: instructure-canvas-courses-api
  description: Show provisional grade status for a student.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/provisional_grades/status
  tags: Courses,Course,Id,Assignments,Assignment,Id,Provisional,Grades,Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesstatus-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesstatus-get-openapi.md
- name: Instructure Canvas Courses API Copy provisional grade
  x-api-slug: instructure-canvas-courses-api
  description: Copy provisional grade.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/provisional_grades/{provisional_grade_id}/copy_to_final_mark
  tags: Courses,Course,Id,Assignments,Assignment,Id,Provisional,Grades,Provisional,Grade,Id,Copy,To,Final,Mark
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idcopy-to-final-mark-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idcopy-to-final-mark-post-openapi.md
- name: Instructure Canvas Courses API Select provisional grade
  x-api-slug: instructure-canvas-courses-api
  description: Select provisional grade.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/provisional_grades/{provisional_grade_id}/select
  tags: Courses,Course,Id,Assignments,Assignment,Id,Provisional,Grades,Provisional,Grade,Id,Select
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idselect-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idselect-put-openapi.md
- name: Instructure Canvas Courses API List assignment submissions
  x-api-slug: instructure-canvas-courses-api
  description: List assignment submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissions-get-openapi.md
- name: Instructure Canvas Courses API Submit an assignment
  x-api-slug: instructure-canvas-courses-api
  description: Submit an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissions-post-openapi.md
- name: Instructure Canvas Courses API Grade or comment on multiple submissions
  x-api-slug: instructure-canvas-courses-api
  description: Grade or comment on multiple submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/update_grades
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,Update,Grades
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsupdate-grades-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsupdate-grades-post-openapi.md
- name: Instructure Canvas Courses API Create Peer Review
  x-api-slug: instructure-canvas-courses-api
  description: Create peer review.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete-openapi.md
- name: Instructure Canvas Courses API Get all Peer Reviews
  x-api-slug: instructure-canvas-courses-api
  description: Get all peer reviews.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get-openapi.md
- name: Instructure Canvas Courses API Create Peer Review
  x-api-slug: instructure-canvas-courses-api
  description: Create peer review.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post-openapi.md
- name: Instructure Canvas Courses API Get a single submission
  x-api-slug: instructure-canvas-courses-api
  description: Get a single submission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-id-get-openapi.md
- name: Instructure Canvas Courses API Grade or comment on a submission
  x-api-slug: instructure-canvas-courses-api
  description: Grade or comment on a submission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-id-put-openapi.md
- name: Instructure Canvas Courses API Upload a file
  x-api-slug: instructure-canvas-courses-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}/comments/files
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id,Comments,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idcommentsfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idcommentsfiles-post-openapi.md
- name: Instructure Canvas Courses API Upload a file
  x-api-slug: instructure-canvas-courses-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}/files
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idfiles-post-openapi.md
- name: Instructure Canvas Courses API Mark submission as unread
  x-api-slug: instructure-canvas-courses-api
  description: Mark submission as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}/read
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idread-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idread-delete-openapi.md
- name: Instructure Canvas Courses API Mark submission as read
  x-api-slug: instructure-canvas-courses-api
  description: Mark submission as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}/read
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idread-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idread-put-openapi.md
- name: Instructure Canvas Courses API Delete an assignment
  x-api-slug: instructure-canvas-courses-api
  description: Delete an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/id
  tags: Courses,Course,Id,Assignments,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsid-delete-openapi.md
- name: Instructure Canvas Courses API Get a single assignment
  x-api-slug: instructure-canvas-courses-api
  description: Get a single assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/id
  tags: Courses,Course,Id,Assignments,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsid-get-openapi.md
- name: Instructure Canvas Courses API Edit an assignment
  x-api-slug: instructure-canvas-courses-api
  description: Edit an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/id
  tags: Courses,Course,Id,Assignments,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idassignmentsid-put-openapi.md
- name: Instructure Canvas Courses API Lists submissions
  x-api-slug: instructure-canvas-courses-api
  description: Lists submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/gradebook_history/date/graders/{grader_id}/assignments/assignment_id/submissions
  tags: Courses,Course,Id,Gradebook,History,Date,Graders,Grader,Id,Assignments,Assignment,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idgradebook-historydategradersgrader-idassignmentsassignment-idsubmissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/coursescourse-idgradebook-historydategradersgrader-idassignmentsassignment-idsubmissions-get-openapi.md
- name: Instructure Canvas Courses API
  x-api-slug: instructure-canvas-courses-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/openapi.md
- name: Instructure Canvas Groups API Redirect to the assignment override for a group
  x-api-slug: instructure-canvas-groups-api
  description: Redirect to the assignment override for a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/assignments/assignment_id/override
  tags: Groups,Group,Id,Assignments,Assignment,Id,Override
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/groupsgroup-idassignmentsassignment-idoverride-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/groupsgroup-idassignmentsassignment-idoverride-get-openapi.md
- name: Instructure Canvas Groups API
  x-api-slug: instructure-canvas-groups-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/openapi.md
- name: Instructure Canvas Sections API Redirect to the assignment override for a
    section
  x-api-slug: instructure-canvas-sections-api
  description: Redirect to the assignment override for a section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{course_section_id}/assignments/assignment_id/override
  tags: Sections,Course,Section,Id,Assignments,Assignment,Id,Override
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionscourse-section-idassignmentsassignment-idoverride-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionscourse-section-idassignmentsassignment-idoverride-get-openapi.md
- name: Instructure Canvas Sections API Get all Peer Reviews
  x-api-slug: instructure-canvas-sections-api
  description: Get all peer reviews.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/peer_reviews
  tags: Sections,Section,Id,Assignments,Assignment,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idpeer-reviews-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idpeer-reviews-get-openapi.md
- name: Instructure Canvas Sections API List assignment submissions
  x-api-slug: instructure-canvas-sections-api
  description: List assignment submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissions-get-openapi.md
- name: Instructure Canvas Sections API Submit an assignment
  x-api-slug: instructure-canvas-sections-api
  description: Submit an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissions-post-openapi.md
- name: Instructure Canvas Sections API Grade or comment on multiple submissions
  x-api-slug: instructure-canvas-sections-api
  description: Grade or comment on multiple submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/update_grades
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,Update,Grades
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsupdate-grades-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsupdate-grades-post-openapi.md
- name: Instructure Canvas Sections API Create Peer Review
  x-api-slug: instructure-canvas-sections-api
  description: Create peer review.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete-openapi.md
- name: Instructure Canvas Sections API Get all Peer Reviews
  x-api-slug: instructure-canvas-sections-api
  description: Get all peer reviews.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get-openapi.md
- name: Instructure Canvas Sections API Create Peer Review
  x-api-slug: instructure-canvas-sections-api
  description: Create peer review.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post-openapi.md
- name: Instructure Canvas Sections API Get a single submission
  x-api-slug: instructure-canvas-sections-api
  description: Get a single submission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{user_id}
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-id-get-openapi.md
- name: Instructure Canvas Sections API Grade or comment on a submission
  x-api-slug: instructure-canvas-sections-api
  description: Grade or comment on a submission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{user_id}
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-id-put-openapi.md
- name: Instructure Canvas Sections API Upload a file
  x-api-slug: instructure-canvas-sections-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{user_id}/files
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,User,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idfiles-post-openapi.md
- name: Instructure Canvas Sections API Mark submission as unread
  x-api-slug: instructure-canvas-sections-api
  description: Mark submission as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{user_id}/read
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,User,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idread-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idread-delete-openapi.md
- name: Instructure Canvas Sections API Mark submission as read
  x-api-slug: instructure-canvas-sections-api
  description: Mark submission as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{user_id}/read
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,User,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idread-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idread-put-openapi.md
- name: Instructure Canvas Sections API
  x-api-slug: instructure-canvas-sections-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/openapi.md
- name: Instructure Canvas Users API List assignments for user
  x-api-slug: instructure-canvas-users-api
  description: List assignments for user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/courses/course_id/assignments
  tags: Users,User,Id,Courses,Course,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/usersuser-idcoursescourse-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/usersuser-idcoursescourse-idassignments-get-openapi.md
- name: Instructure Canvas Users API
  x-api-slug: instructure-canvas-users-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/openapi.md
- name: Instructure Canvas Utility APIs Retrieve assignments enabled for grade export
    to SIS
  x-api-slug: instructure-canvas-utility-apis
  description: Retrieve assignments enabled for grade export to sis.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//api/sis/accounts/{account_id}/assignments
  tags: Api,Sis,Accounts,Account,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/apisisaccountsaccount-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/apisisaccountsaccount-idassignments-get-openapi.md
- name: Instructure Canvas Utility APIs Retrieve assignments enabled for grade export
    to SIS
  x-api-slug: instructure-canvas-utility-apis
  description: Retrieve assignments enabled for grade export to sis.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//api/sis/courses/{course_id}/assignments
  tags: Api,Sis,Courses,Course,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/apisiscoursescourse-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/apisiscoursescourse-idassignments-get-openapi.md
- name: Instructure Canvas Utility APIs
  x-api-slug: instructure-canvas-utility-apis
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Assignments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/assignments/master/_listings/instructure/openapi.md
x-common:
- type: x-blog
  url: http://blog.instructure.com
- type: x-blog-rss
  url: http://voice.instructure.com/CMS/UI/Modules/BizBlogger/rss.aspx?tabid=772438&moduleid=1638884&maxcount=25&t=415c2e5d197a4d6f7cdcc81385b677f1
- type: x-crunchbase
  url: https://crunchbase.com/organization/instructure
- type: x-crunchbase
  url: http://www.crunchbase.com/company/instructure
- type: x-email
  url: info@instructure.com
- type: x-email
  url: jobs@instructure.com
- type: x-email
  url: privacy@instructure.com
- type: x-email
  url: legal@instructure.com
- type: x-github
  url: https://github.com/instructure
- type: x-twitter
  url: https://twitter.com/instructure
- type: x-website
  url: http://instructure.com
- type: x-website
  url: https://canvas.instructure.com/doc/api/index.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---