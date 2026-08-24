# San Diego probate card art

Rendered postcard images, published so thanks.io can fetch them. Their API
takes image **URLs**, not uploads, and the repository that builds these is
private.

Nothing here is written by hand. `publish_images.py` in the build
repository renders the art and pushes it, filed by the day it was mailed:

    cards/YYYY-MM-DD/fronts/<case number>_front.png
    cards/YYYY-MM-DD/back-<option>.png

Anything older than two weeks is deleted on the next run.

## What is in these images

The fronts carry a case number, the court's own case name, party surnames,
the filed year, the next hearing date and the docket flags. Every one of
those is published by the San Diego Superior Court on its daily probate
calendar.

The backs carry no case data at all.

No attorney name, address or phone number appears on a card. Neither does
any property value or real-estate assessment. Those exist in the mailing
list and in the order sent to thanks.io, and neither of those is public.
