# MediaEvent

## Description

Base for all events raised by elements in the Kurento media server

## Data Model

+ `id` : Entity's unique identifier.

+ `type` : Entity type. It must be equal to `MediaEvent`

+ `eventType` : Type of event that was raised.
    + Attribute type: [Text](https://schema.org/Text)
    + Mandatory

+ `timestamp` : Time when event raised.
    + Attribute type: [DateTime](https://schema.org/DateTime)
    + Mandatory

+ `source` : Object´s technical information that raised the event
    + Attribute type: [StructuredValue](http://schema.org/StructuredValue)
    + Optional

+ `refSeeAlso` : Reference to one related entities that may provide extra, specific information about this Media Event
    + Attribute type: Reference.
    + Optional

## Example

    {
      "id": "mediaEvent:1509702324600",
      "type": "MediaEvent",
      "eventType": "plate-detected",
      "source": {
        "name": "03ea110c-0ab2-4b19-8618-57f474721c86_kurento.MediaPipeline/28e4ae84-4e96-43bb-a812-538f7950b75f_platedetector.PlateDetectorFilter",
        "creationTime": "2017-11-03T10:45:19Z",
        "sendTagsInEvents": false,
        "parent": {
          "name": "03ea110c-0ab2-4b19-8618-57f474721c86_kurento.MediaPipeline",
          "creationTime": "2017-11-03T10:45:19Z",
          "sendTagsInEvents": false
        }
      },
      "timestamp": "2017-11-03T10:45:23Z"
    }


## Test it with a real service

T.B.D.

## Issues
