---
swagger: "2.0"
x-collection-name: AWS Machine Learning
x-complete: 0
info:
  title: AWS Machine Learning API Delete Evaluation
  version: 1.0.0
  description: Assigns the DELETED status to an Evaluation, rendering it unusable.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteBatchPrediction:
    get:
      summary: Delete Batch Prediction
      description: Assigns the DELETED status to a BatchPrediction, rendering it unusable.
      operationId: deleteBatchPrediction
      x-api-path-slug: actiondeletebatchprediction-get
      parameters:
      - in: query
        name: BatchPredictionId
        description: A user-supplied ID that uniquely identifies the BatchPrediction
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Batches
  /?Action=DeleteDataSource:
    get:
      summary: Delete Data Source
      description: Assigns the DELETED status to a DataSource, rendering it unusable.
      operationId: deleteDataSource
      x-api-path-slug: actiondeletedatasource-get
      parameters:
      - in: query
        name: DataSourceId
        description: A user-supplied ID that uniquely identifies the DataSource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Data Sources
  /?Action=DeleteEvaluation:
    get:
      summary: Delete Evaluation
      description: Assigns the DELETED status to an Evaluation, rendering it unusable.
      operationId: deleteEvaluation
      x-api-path-slug: actiondeleteevaluation-get
      parameters:
      - in: query
        name: EvaluationId
        description: A user-supplied ID that uniquely identifies the Evaluation to
          delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Evaluations
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