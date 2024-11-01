# Inlämningsuppgift 3 - AWS Serverless applikation. 
Steg
1. Läs igenom uppgiften och lägg till fler steg
2. Bryt ner stegen i så små delar som möjligt
3. Skriv ner vad som har gjorts i varje steg för dokumentationen senare.
Skapade en S3 bucket för projektet
  la in en fil som heter index.html och satte den som static website host längst ner i bucket permissions
Skapade en användare för github att använda arn:aws:iam::767397794379:user/github-aws3-serverless-s3access med lösen AmazonS3-GithubCICD
Skapade en roll för github att använda CICD med permission AmazonS3FullAccess
La in Trust relationship
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Principal": {
                "AWS": "arn:aws:iam::767397794379:user/github-aws3-serverless-s3access"
            },
            "Action": "sts:AssumeRole"
        }
    ]
}
på rollen 
Gick till användaren och skapade access keys för en applikation utanför AWS och la till det som secrets i github under AWS_ACCESS_KEY_ID och AWS_SECRET_ACCESS_KEY
### Index
1. [Inledning](#inledning)
2. [Krav](#krav)
3. [Systemarkitektur - Översikt](#systemarkitektur---översikt)
	- [Komponenter](#komponenter)
	- [Utnyttjade molntjänster](#utnyttjade-molntjänster)
1. [Provisionering av driftmiljö och driftsättning av applikation](#provisionering-av-driftmiljö-och-driftsättning-av-applikation)
2. [Slutsats](#slutsats)
3. [Appendix](#appendix)
4. [Referenser](#referenser)
### Verktyg och tjänster

## Inledning

## Krav
Denna uppgiften kräver en fungerande och skalbar webbapplikation I AWS serverless infrastrukturen. Samt redögöra för vilka molntjänster man har använt, vilket syfte dem har och dokumentera processen av att sätta upp applikationen.
## Systemarkitektur - Översikt

### Komponenter

### Utnyttjade molntjänster

## Provisionering av driftmiljö och driftsättning av applikation

## Slutsats

## Appendix

## Referenser