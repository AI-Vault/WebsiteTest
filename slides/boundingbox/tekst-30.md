# Non Max Suppression (NMS)

## Probleem
- Het algoritme vindt meerdere bounding boxes per object. Dit kan leiden tot verwarring en inefficiëntie bij objectdetectie.

## Oplossing is NMS
- Selecteer de box met de hoogste waarschijnlijkheid (confidence score).
- Suppress (onderdruk) alle andere boxes met een Intersection over Union (IOU) groter dan 0.5. 

NMS helpt bij het beperken van overlappende detecties en zorgt ervoor dat we een enkele, nauwkeurige voorspelling per object behouden.