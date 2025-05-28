# Sliding Window Algorithm

- Je beweegt een window over het plaatje heen en laat het getrainde model bepalen of er iets zit.
- Hiermee krijg je wat er zit, en ook de locatie en bounding boxes.
- Maar dit is sequentieel en daarom erg langzaam.
- Je kan dit ook allemaal in één keer berekenen door het op te zetten als een Conv Net. Dan kan je alles sliding windows in één keer berekenen = YOLO.