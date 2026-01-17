FROM alpine:latest

# Installiere benötigte Pakete
RUN apk add --no-cache bash curl

# Kopiere den Treiber und Skripte
COPY setup.sh /setup.sh
COPY /eGTouch64 /usr/local/bin/lin-touch

# Berechtigungen setzen
RUN chmod +x /setup.sh /usr/local/bin/lin-touch

# Startbefehl
CMD ["/setup.sh"]