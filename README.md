# ![LOGO](logo.png) xworks API **flow**ground Connector

## Description

A generated **flow**ground connector for the xworks API API (version v1).

Generated from: https://dev.api.xworks.net/rest/1<br/>
Generated at: 2019-07-01T17:54:54+03:00

## API Description



## Authorization

This API does not require authorization.

## Actions

### Erzeugt einen Token fur die weitere Verwendung der API

*Tags:* `Auth`

### Entfernt den Token aus dem System (Kommt einer Abmeldung gleich)

*Tags:* `Auth`

### Verlangert den Token um die angegebenen Tage

*Tags:* `Auth`

#### Input Parameters
* `validDays` - _required_ - Anzahl der Tage, um die der Token verlangert werden soll. Wenn validDays nicht angegeben wird, so wird der Token um die ursprunglich angegebene Anzahl der Tage verlangert.
* `info` - _optional_ - Die Information, welche bei dem Token angegeben werden soll (Optional)

### Erzeugt einen Token fur einen zugehorigen (Team) Account und fur die weitere Verwendung der API

*Tags:* `Auth`

### Ermittelt alle Termine des Benutzers aus einem Kalenderverzeichnis. Sollte kein KalenderVerzeichnis angegeben werden, so werden alle Termine zuruckgegeben.

*Tags:* `Calendar`

#### Input Parameters
* `folderId` - _optional_ - Id des Kalenderverzeichnisses, aus dem die Termine ermittelt werden sollen. Sollte keine Verzeichnis-Id angegeben werden, so werden alle Termine zuruckgegeben.

### Ermittelt alle Informationen zu einem Termin

*Tags:* `Calendar`

#### Input Parameters
* `appointmentId` - _required_ - Id des Termins, dessen Informationen ermittelt werden sollen

### Erstellt einen neuen einfachen Termin

*Tags:* `Calendar`

### Erstellt eine tagliche Terminserie

*Tags:* `Calendar`

### Erstellt eine wochentliche Terminserie

*Tags:* `Calendar`

### Erstellt eine monatliche Terminserie

*Tags:* `Calendar`

### Erstellt eine jahrliche Terminserie

*Tags:* `Calendar`

### Erstellt eine Ausnahme zu einer Terminserie

*Tags:* `Calendar`

### Aktualisiert einen einfachen Termin

*Tags:* `Calendar`

### Aktualisiert einen taglichen Termin

*Tags:* `Calendar`

### Aktualisiert einen wochentlichen Termin

*Tags:* `Calendar`

### Aktualisiert einen monatlichen Termin

*Tags:* `Calendar`

### Aktualisiert einen jahrlichen Termin

*Tags:* `Calendar`

### Loscht mehere Termine

*Tags:* `Calendar`

### Liefert die Informationen Dateianzahl, Speichergrosse und genutzten Speicher

*Tags:* `Cloud`

### Ermittelt die Verzeichnisse des Benutzers

*Tags:* `Cloud`

#### Input Parameters
* `parentId` - _optional_ - Id des Verzeichnisses, dessen direkte Unterverzeichnisse ermittelt werden sollen.
* `showArchiveFolders` - _optional_ - Gibt an, ob Archivordner mit angezeigt werden sollen

### Liefert Informationen eines Verzeichnisses

*Tags:* `Cloud`

#### Input Parameters
* `id` - _required_ - Id des Verzeichnisses

### Liefert die Volltext-Daten einer Datei

*Tags:* `Cloud`

#### Input Parameters
* `id` - _required_ - Id der Datei

### Liefert das EventLog eines Objektes

*Tags:* `Cloud`

#### Input Parameters
* `objectId` - _required_ - Object-ID
* `startValue` - _optional_ - Startdatum
* `limit` - _optional_ - Anzahl der zuruckzugebenden Events
* `isSortDesc` - _optional_ - Sortierung

### Erstellt ein Verzeichnis

*Tags:* `Cloud`

### Loscht ein Verzeichnis

*Tags:* `Cloud`

#### Input Parameters
* `id` - _required_ - Id des zu loschenden Verzeichnisses
* `force` - _optional_

### Bennennt ein Verzeichnis um

*Tags:* `Cloud`

### Verschiebt ein Verzeichnis

*Tags:* `Cloud`

### Andert die Kategorie eines Verzeichnis

*Tags:* `Cloud`

### Markiert ein Verzeichnis als Favorit

*Tags:* `Cloud`

### Offline-Verfugbarkeit andern

*Tags:* `Cloud`

### Archivierung eines Ordners vornehmen

*Tags:* `Cloud`

### Ermittelt alle Dateien des Benutzers, die der Suche entsprechen

*Tags:* `Cloud`

### Ermittelt alle Dateien des Benutzers aus einem Verzeichnis

*Tags:* `Cloud`

### Ermittelt alle Dateien des Benutzers die sich seit dem ubergebenen Datum geandert haben

*Tags:* `Cloud`

### Ermittelt alle Dateien des Benutzers die sich seit dem ubergebenen Datum geandert haben

*Tags:* `Cloud`

### Liefert Informationen zu einer Datei

*Tags:* `Cloud`

#### Input Parameters
* `id` - _required_
* `crcFlags` - _optional_

### Loscht eine Datei

*Tags:* `Cloud`

### Bennennt eine Datei um

*Tags:* `Cloud`

### Verschiebt eine Datei

*Tags:* `Cloud`

### Wiederherstellung einer Datei aus dem Papierkorb in das urprungliche Verzeichnis

*Tags:* `Cloud`

### Anderung von Dateiattributen

*Tags:* `Cloud`

### Markiert ein Datei als Favorit

*Tags:* `Cloud`

### Offline-Verfugbarkeit andern

*Tags:* `Cloud`

### Kopiert eine Datei

*Tags:* `Cloud`

### Kopiert den Anhang einer Nachricht in die Cloud

*Tags:* `Cloud`

### Liefert das Bild in den angeforderten Abmessungen

*Tags:* `Cloud`

#### Input Parameters
* `id` - _required_ - Id des Bildes
* `width` - _optional_ - Weite (optional)
* `height` - _optional_ - Hohe (optional)

### Liefert das Bild als Thumbnail aus. Wenn keine Weite und Hohe ubergeben wird, dann wird das Thumbnail in 240x240px ausgeliefert.

*Tags:* `Cloud`

#### Input Parameters
* `id` - _required_ - Id des Bildes
* `width` - _optional_ - Weite (optional)
* `height` - _optional_ - Hohe (optional)

### Liefert das Bild als Vorschau mit max. 1280px in Weite oder Hohe aus

*Tags:* `Cloud`

#### Input Parameters
* `id` - _required_ - Id des Bildes
* `width` - _optional_ - Weite (optional)
* `height` - _optional_ - Hohe (optional)

### Erzeugen eines Sharinglink

*Tags:* `Cloud`

### Loschen einses Sharinglinks

*Tags:* `Cloud`

### Erzeugen eines Sharinglinks

*Tags:* `Cloud`

### Loschen einses Sharinglinks

*Tags:* `Cloud`

### Liefert die Streaming-Url

*Tags:* `Cloud`

#### Input Parameters
* `id` - _required_ - Id der Videos oder Audio Datei
* `resolution` - _optional_ - 360 oder 720 (optional)

### Hochladen einer Datei

*Tags:* `Cloud`

#### Input Parameters
* `folderId` - _required_ - Id des Verzeichnisses
* `fileName` - _optional_
* `fileId` - _optional_
* `created` - _optional_
* `modified` - _optional_
* `option` - _optional_
* `crcFlags` - _optional_

### Download einer Datei

*Tags:* `Cloud`

#### Input Parameters
* `fileId` - _required_ - Id des Datei
* `appId` - _optional_
* `devId` - _optional_
* `token` - _optional_
* `langId` - _optional_

### Ermittelt alle Kontakte des Benutzers aus einem Verzeichnis. Sollte kein Verzeichnis angegeben werden, so werden alle Kontakte zuruckgegeben.

*Tags:* `Contact`

#### Input Parameters
* `folderId` - _optional_ - Id des Verzeichnisses, aus dem die Kontakte ermittelt werden sollen. Sollte keine Verzeichnis-Id angegeben werden, so werden alle Kontakte zuruckgegeben.
* `imageSize` - _optional_ - Grosse des Kontaktbildes, welches als imageUrl zuruckgegeben werden soll, sofern ein Kontaktbild vorhanden ist
    Possible values: 0, 1, 2.

### Ermittelt alle Informationen zu einem Kontakt

*Tags:* `Contact`

#### Input Parameters
* `contactId` - _required_ - Id des Kontaktes, dessen Informationen ermittelt werden sollen
* `imageSize` - _optional_ - Grosse des Kontaktbildes, welches als imageUrl zuruckgegeben werden soll, sofern ein Kontaktbild vorhanden ist
    Possible values: 0, 1, 2.

### Erstellt einen neuen Kontakt

*Tags:* `Contact`

### Loscht einen Kontakt

*Tags:* `Contact`

#### Input Parameters
* `contactId` - _required_ - Id des Kontaktes, welcher geloscht werden soll

### Verschiebt Kontakte in ein Verzeichnis

*Tags:* `Contact`

### Andert einen Kontakt

*Tags:* `Contact`

### Ladt ein Bild zu einem Kontakt hoch

*Tags:* `Contact`

### Ladt das Bild eines Kontaktes herunter, sofern der Kontakt ein Bild besitzt

*Tags:* `Contact`

#### Input Parameters
* `contactId` - _required_ - Id des Kontaktes
* `size` - _required_ - Gewunschte Grosse des Bildes
    Possible values: 0, 1, 2.

### Ermittelt alle zugehorigen Konten zu dem aktuellem Benutzer

*Tags:* `Customer`

### Ermittelt alle benotigten Informationen zu dem aktuellem Benutzer

*Tags:* `Customer`

#### Input Parameters
* `filter` - _optional_ - Angabe der gewunschten Daten
    Possible values: 1, 2, 4, 8, 16, 32, 64, 127.
* `clientId` - _optional_

### Ermittelt das Icon zu einem Modul

*Tags:* `Customer`

#### Input Parameters
* `moduleId` - _required_ - UID des Moduls, dessen Icon zuruckgegeben werden soll
* `clientId` - _optional_

### Ermittelt die Einstellungen zu einem Modul

*Tags:* `Customer`

#### Input Parameters
* `moduleId` - _required_ - UID des Moduls, dessen Einstellungen zuruckgegeben werden soll
* `clientId` - _optional_

### Liefert eine Liste mit allen moglichen Domainnamen fur Emailadressen zuruck

*Tags:* `Customer`

### Ermittelt das Guthaben des Benutzers

*Tags:* `Customer`

### Ermittelt alle Informationen zu dem primaren Kontakt des Benutzers

*Tags:* `Customer`

### Andert den primaren Kontakt des Benutzers

*Tags:* `Customer`

### Ermittelt die Logbucheintrage des Benutzers

*Tags:* `Customer`

### Erstellt einen neuen Logbucheintrag

*Tags:* `Customer`

### Startet die Passwort-Vergessen-Funktionalitat und ermittelt die Sicherheitsfrage

*Tags:* `Customer`

### Uberpruft die angegebene Antwort der Sicherheitsfrage in der Passwort-Vergessen-Funktionalitat

*Tags:* `Customer`

### Ruft die Widgets des Benutzers ab

*Tags:* `Dashboard`

#### Input Parameters
* `folderId` - _required_ - Id des Verzeichnisses aus dem die Widgets ermittelt werden sollen
* `filter` - _optional_
    Possible values: 1, 2, 3.

### Ruft die Widgets fur die Startanzeige des Benutzers ab

*Tags:* `Dashboard`

### Ruft die Informationen zu einem Widget ab

*Tags:* `Dashboard`

#### Input Parameters
* `widgetId` - _required_ - Id des Widgets, dessen Informationen ermittelt werden sollen
* `typeId` - _optional_ - Typ des Widgets (Optional - Wenn nicht angegeben, wird der WidgetTyp NOTE angenommen)
    Possible values: 4, 14.

### Aktualisiert ein Widget

*Tags:* `Dashboard`

### Loscht ein Widget

*Tags:* `Dashboard`

#### Input Parameters
* `widgetId` - _required_ - Id des zu loschenden Widgets
* `typeId` - _optional_ - Typ des Widgets (Optional - Wenn nicht angegeben, wird der WidgetTyp NOTE angenommen)
    Possible values: 4, 14.

### Loscht die angegebene Widgetliste

*Tags:* `Dashboard`

### Erstellt ein Widgets

*Tags:* `Dashboard`

### Verschiebt ein Widget in ein Verzeichnis

*Tags:* `Dashboard`

### Verschiebt eine Liste von Widgets in ein Verzeichnis

*Tags:* `Dashboard`

### Markiert eine Liste von Widgets als Favoriten

*Tags:* `Dashboard`

### Ermittelt die Verzeichnisse des Benutzers

*Tags:* `Directory`

#### Input Parameters
* `typeId` - _optional_ - Typ der Verzeichnisse, die ermittelt werden sollen
    Possible values: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 20.
* `moduleId` - _optional_ - Modul, fur das die Verzeichnisse ermittelt werden sollen
    Possible values: 0, 1, 2, 3, 4, 5, 6, 7, 8.
* `folderId` - _optional_ - Id des Verzeichnisses, dessen direkte Unterverzeichnisse ermittelt werden sollen.

### Erstellt ein Verzeichnis

*Tags:* `Directory`

### Loscht ein Verzeichnis

*Tags:* `Directory`

#### Input Parameters
* `folderId` - _required_ - Id des zu loschenden Verzeichnisses

### Bennennt ein Verzeichnis um

*Tags:* `Directory`

### Verschiebt ein Verzeichnis

*Tags:* `Directory`

### Ermittelt die Status von Verzeichnissen

*Tags:* `Directory`

#### Input Parameters
* `moduleId` - _optional_ - Modul, fur dessen Verzeichnisse die Status ermittelt werden sollen
    Possible values: 0, 1, 2, 3, 4, 5, 6, 7, 8.

### Ermittelt alle externen IMAP-Konten des Benutzers

*Tags:* `ExternalMail`

### Fugt ein neues externes Konto hinzu

*Tags:* `ExternalMail`

### Aktualisiert ein externes Konto

*Tags:* `ExternalMail`

#### Input Parameters
* `accountId` - _required_ - ID des externen Kontos

### Loscht ein extenes Konto

*Tags:* `ExternalMail`

#### Input Parameters
* `accountId` - _required_ - ID des externen Kontos

### Validiert ein externes Konto

*Tags:* `ExternalMail`

### Ermittelt die IMAP-Verzeichnisse des Benutzers

> Der <code>EMS-ACCOUNT-ID</code>-Header muss ubermittelt werden

*Tags:* `ExternalMail`

### Erstellt ein Verzeichnis

> Der <code>EMS-ACCOUNT-ID</code>-Header muss ubermittelt werden

*Tags:* `ExternalMail`

### Bennennt ein Verzeichnis um

> Der <code>EMS-ACCOUNT-ID</code>-Header muss ubermittelt werden

*Tags:* `ExternalMail`

### Verschiebt ein Verzeichnis

> Der <code>EMS-ACCOUNT-ID</code>-Header muss ubermittelt werden

*Tags:* `ExternalMail`

### Loscht ein Verzeichnis

> Der <code>EMS-ACCOUNT-ID</code>-Header muss ubermittelt werden

*Tags:* `ExternalMail`

#### Input Parameters
* `folderId` - _required_ - Id des zu loschenden Verzeichnisses

### Ermittelt die Nachrichten des Benutzers

> Der <code>EMS-ACCOUNT-ID</code>-Header und der <code>EMS-FOLDER-ID-Header</code> mussen ubermittelt werden

*Tags:* `ExternalMail`

### Liefert die vollstandigen Daten einer Nachricht

> Der <code>EMS-ACCOUNT-ID</code>-Header und der <code>EMS-FOLDER-ID-Header</code> mussen ubermittelt werden

*Tags:* `ExternalMail`

#### Input Parameters
* `messageId` - _required_ - Id der Nachricht
* `filter` - _optional_ - Filter fur den Inhalt der Nachricht
    Possible values: 0, 1, 2, 4, 8, 16, 24, 25, 32, 64, 89.

### Ermittelt eine Vorschau des Textes einer Nachricht

> Der <code>EMS-ACCOUNT-ID</code>-Header und der <code>EMS-FOLDER-ID-Header</code> mussen ubermittelt werden

*Tags:* `ExternalMail`

#### Input Parameters
* `messageId` - _required_ - Id der Nachricht
* `length` - _optional_ - Gewunschte Lange der Vorschau (Anzahl Zeichen). Eine Angabe von 10 bis 1024 Zeichen ist moglich. Wird kein Wert angegeben, so werden maximal 512 Zeichen ausgegeben.

### Ermittelt den Header einer Nachricht

> Der <code>EMS-ACCOUNT-ID</code>-Header und der <code>EMS-FOLDER-ID-Header</code> mussen ubermittelt werden

*Tags:* `ExternalMail`

#### Input Parameters
* `messageId` - _required_ - Id der Nachricht, deren Header ermittelt werden sollen

### Erzeugt eine Nachricht

> Der <code>EMS-ACCOUNT-ID</code>-Header und der <code>EMS-FOLDER-ID-Header</code> mussen ubermittelt werden

*Tags:* `ExternalMail`

### Speichert eine Nachricht als Entwurf

> Der <code>EMS-ACCOUNT-ID</code>-Header und der <code>EMS-FOLDER-ID-Header</code> mussen ubermittelt werden

*Tags:* `ExternalMail`

### Loscht Nachrichten

> Der <code>EMS-ACCOUNT-ID</code>-Header und der <code>EMS-FOLDER-ID-Header</code> mussen ubermittelt werden

*Tags:* `ExternalMail`

### Verschiebt Nachrichten in ein Verzeichnis

> Der <code>EMS-ACCOUNT-ID</code>-Header und der <code>EMS-FOLDER-ID-Header</code> mussen ubermittelt werden

*Tags:* `ExternalMail`

### Aktualisiert den Status von Nachrichten

> Der <code>EMS-ACCOUNT-ID</code>-Header und der <code>EMS-FOLDER-ID-Header</code> mussen ubermittelt werden

*Tags:* `ExternalMail`

### Ermittelt den Anhang einer Nachricht

> Der <code>EMS-ACCOUNT-ID</code>-Header und der <code>EMS-FOLDER-ID-Header</code> mussen ubermittelt werden

*Tags:* `ExternalMail`

#### Input Parameters
* `messageId` - _required_ - Id der Nachricht, deren Anhang zuruckgegeben werden soll
* `attachmentId` - _required_ - Id des Anhangs, welcher zuruckgegeben werden soll

### Sucht nach Nachrichten

> Liefert immer eine leere Liste, da die Suche uber IMAP noch nicht unterstutzt wird.<br/>
> Der <code>EMS-ACCOUNT-ID</code>-Header und der <code>EMS-FOLDER-ID-Header</code> mussen ubermittelt werden

*Tags:* `ExternalMail`

### Ermittelt alle Lesezeichen des Benutzers aus einem Verzeichnis. Sollte kein Verzeichnis angegeben werden, so werden alle Lesezeichen zuruckgegeben.

*Tags:* `Favorite`

#### Input Parameters
* `folderId` - _optional_ - Id des Verzeichnisses, aus dem die Lesezeichen ermittelt werden sollen. Sollte keine Verzeichnis-Id angegeben werden, so werden alle Lesezeichen zuruckgegeben.

### Ermittelt alle Informationen zu einem Lesezeichen

*Tags:* `Favorite`

#### Input Parameters
* `bookmarkId` - _required_ - Id des lesezeichens, dessen Informationen ermittelt werden sollen

### Erstellt einen neues Lesezeichen

*Tags:* `Favorite`

### Loscht Lesezeichen

*Tags:* `Favorite`

### Verschiebt Lesezeichen in ein Verzeichnis

*Tags:* `Favorite`

### Andert ein Lesezeichen

*Tags:* `Favorite`

### Liefert das Impressum des angegebenen Providers

*Tags:* `Legal`

#### Input Parameters
* `providerId` - _optional_ - Id des Providers, dessen Impressum ermittelt werden soll

### Liefert die AGB des angegebenen Providers

*Tags:* `Legal`

#### Input Parameters
* `providerId` - _optional_ - Id des Providers, dessen AGB ermittelt werden soll

### Liefert die Datenschutzerklarung des angegebenen Providers

*Tags:* `Legal`

#### Input Parameters
* `providerId` - _optional_ - Id des Providers, dessen Datenschutzerklarung ermittelt werden soll

### Liefert die Lizenzinformationen des angegebenen Providers

*Tags:* `Legal`

#### Input Parameters
* `providerId` - _optional_ - Id des Providers, dessen Lizenzinformationen ermittelt werden soll

### Ermittelt die Nachrichten des Benutzers

*Tags:* `Mailbox`

#### Input Parameters
* `folderId` - _optional_ - Id des Verzeichnisses aus dem die Nachrichten ermittelt werden sollen. Wenn kein Verzeichnis angegeben wird, so werden alle Nachrichten ermittelt
* `filter` - _optional_ - Der Nachrichtenfilter, welcher festlegt welche Nachrichtentypen ermittelt werden sollen
    Possible values: 0, 1, 2, 3, 4, 8, 16, 32, -1.

### Liefert die vollstandigen Daten einer Nachricht

*Tags:* `Mailbox`

#### Input Parameters
* `messageId` - _required_ - Id der Nachricht
* `filter` - _optional_ - Filter fur den Inhalt der Nachricht
    Possible values: 0, 1, 2, 4, 8, 16, 24, 25, 32, 64, 89.
* `index` - _optional_ - Index der Seite, die bei einem Fax angezeigt werden soll. Der Wert 0 zeigt eine Ubersicht mit Thumbnails an. Dieser Wert wird nur bei einer Fax-Nachricht ausgewertet.
* `zoom` - _optional_ - Zoom der Fax-Seite. Dieser Wert wird nur bei einer Fax-Nachricht ausgewertet und auch nur dann, wenn ein Seiten-Index grosser 0 angegeben wurde.

### Ermittelt eine Vorschau des Textes einer Nachricht

*Tags:* `Mailbox`

#### Input Parameters
* `messageId` - _required_ - Id der Nachricht
* `length` - _optional_ - Gewunschte Lange der Vorschau (Anzahl Zeichen). Eine Angabe von 10 bis 1024 Zeichen ist moglich. Wird kein Wert angegeben, so werden maximal 512 Zeichen ausgegeben.

### Ermittelt den Header einer Nachricht

*Tags:* `Mailbox`

#### Input Parameters
* `messageId` - _required_ - Id der Nachricht, deren Header ermittelt werden sollen

### Erzeugt eine Nachricht

*Tags:* `Mailbox`

### Speichert eine Nachricht als Entwurf

*Tags:* `Mailbox`

### Erzeugt eine SMS

*Tags:* `Mailbox`

### Erzeugt eine VoiceMail

*Tags:* `Mailbox`

### Erzeugt eine MMS

*Tags:* `Mailbox`

### Erzeugt ein Fax

*Tags:* `Mailbox`

### Erstellt eine Expressantwort auf eine vorher empfangene Email

*Tags:* `Mailbox`

### Loscht Nachrichten

*Tags:* `Mailbox`

### Verschiebt Nachrichten in ein Verzeichnis

*Tags:* `Mailbox`

### Aktualisiert den Status von Nachrichten

*Tags:* `Mailbox`

### Ermittelt den Anhang einer Nachricht

*Tags:* `Mailbox`

#### Input Parameters
* `messageId` - _required_ - Id der Nachricht, deren Anhang zuruckgegeben werden soll
* `attachmentId` - _required_ - Id des Anhangs, welcher zuruckgegeben werden soll

### Sucht nach Nachrichten

*Tags:* `Mailbox`

### Register

*Tags:* `Notify`

### Unregister

*Tags:* `Notify`

### Update

*Tags:* `Notify`

### Poi_GetFolder

*Tags:* `Poi`

#### Input Parameters
* `uid` - _required_

### Poi_GetContent

*Tags:* `Poi`

#### Input Parameters
* `uid` - _required_
* `id` - _required_
* `imageSize` - _optional_
    Possible values: 0, 1, 2.

### Poi_GetImage

*Tags:* `Poi`

### Ermittelt alle Emailadressen des Benutzers

*Tags:* `Settings`

#### Input Parameters
* `addressType` - _optional_ - Legt fest, welche Emailadressen ermittelt werden sollen
    Possible values: 0, 1, 2, 3, 4.

### Legt eine neue Alias-Emailadresse an

*Tags:* `Settings`

### Legt eine neue Emailadresse an, welche nur eine bestimmte Lebensdauer aufweist

*Tags:* `Settings`

#### Input Parameters
* `lifeTime` - _optional_
    Possible values: 0, 1, 2, 3.

### Loscht Emailaddressen des Benutzers

*Tags:* `Settings`

### Ermittelt alle Mailboxen (SubAccounts), die dieser Account verwaltet.

*Tags:* `Settings`

### Erstellt ein neues Postfach (SubAccount)

*Tags:* `Settings`

### Loscht ein Postfach (SubAccount)

*Tags:* `Settings`

### Gibt eine Liste mit moglichen Nummern fur die Telefon- und Faxeinstellungen zuruck

*Tags:* `Settings`

#### Input Parameters
* `count` - _required_ - Anzahl der gewunschten Nummern

### Ermittelt alle Telefon- und Faxeinstellungen

*Tags:* `Settings`

### Erstellt eine neue Telefon- bzw. Faxeinstellung

*Tags:* `Settings`

### Loscht Telefon- bzw. Faxeinstellungen

*Tags:* `Settings`

### Aktualisiert Telefon- bzw. Faxeinstellungen

*Tags:* `Settings`

### Ermittelt alle authentifizierten Adressen

*Tags:* `Settings`

### Validiert (pruft) eine authentifizierte Adresse

*Tags:* `Settings`

#### Input Parameters
* `addressId` - _required_ - Id der Adresse, welche validiert (gepruft) werden soll
* `key` - _required_ - Schlussel, mit dem die Prufung der Adresse abgeschlossen werden kann

### Erstellt eine zu authentifizierende Adresse

*Tags:* `Settings`

### Loscht eine authentifizierte Adresse

*Tags:* `Settings`

#### Input Parameters
* `addressId` - _required_ - Id der Adresse, welche geloscht werden soll

### Ermittelt alle POP3-Sammeldienste des Benutzers

*Tags:* `Settings`

### Erstellt einen neuen POP3-Sammeldienst

*Tags:* `Settings`

### Aktualisiert einen POP3-Sammeldienst

*Tags:* `Settings`

### Loscht eine Reihe von POP3-Sammeldiensten

*Tags:* `Settings`

### Ermittelt alle Signaturen des Benutzers

*Tags:* `Settings`

### Erstellt eine neue Signatur

*Tags:* `Settings`

### Aktualisiert eine Signatur

*Tags:* `Settings`

### Loscht eine Reihe von Signaturen

*Tags:* `Settings`

### Ermittelt die Einstellungen des Benutzers

*Tags:* `Settings`

### Aktualisiert die Einstellungen des Benutzers

*Tags:* `Settings`

### Aktualisiert die erweiterten Einstellungen des Benutzers

*Tags:* `Settings`

### Aktualisiert das Sicherheitspasswort des Benutzers

*Tags:* `Settings`

### Aktualisiert den Sicherheits-PIN des Benutzers

*Tags:* `Settings`

### Aktualisiert die Sicherheitsfrage des Benutzers

*Tags:* `Settings`

### Ermittelt die Nachrichtenregeln des Benutzers

*Tags:* `Settings`

### Ermittelt eine Nachrichtenregel

*Tags:* `Settings`

#### Input Parameters
* `ruleId` - _optional_ - Id der Nachrichtenregel, deren Informationen abgerufen werden sollen

### Erstellt eine neue Nachrichtenregel

*Tags:* `Settings`

### Erstellt eine neue Nachrichtenregel, die Nachrichten in ein Verzeichnis verschiebt

*Tags:* `Settings`

### Erstellt eine neue Nachrichtenregel, die Nachrichten weiterleitet

*Tags:* `Settings`

### Erstellt eine neue Nachrichtenregel, die Benachrichtigungen uber den Erhalt von Nachrichten versendet

*Tags:* `Settings`

### Aktualisiert eine Nachrichtenregel

*Tags:* `Settings`

### Aktualisiert eine Nachrichtenregel, die Nachrichten in ein Verzeichnis verschiebt

*Tags:* `Settings`

### Aktualisiert eine Nachrichtenregel, die Nachrichten weiterleitet

*Tags:* `Settings`

### Aktualisiert eine Nachrichtenregel, die Benachrichtigungen uber den Erhalt von Nachrichten versendet

*Tags:* `Settings`

### Loscht eine Reihe von Nachrichtenregeln

*Tags:* `Settings`

### Aktiviert eine Nacrichtenregel

*Tags:* `Settings`

#### Input Parameters
* `ruleId` - _optional_ - Id der Nachrichrenregel, welche aktiviert werden soll

### Deaktiviert eine Nachrichtenregel

*Tags:* `Settings`

#### Input Parameters
* `ruleId` - _optional_ - Id der Nachrichtenregel, welche deaktiviert werden soll

### Erstellt eine neue Regel fur Spamnachrichten

*Tags:* `Settings`

### Erstellt eine Regel fur Spamnachrichten

*Tags:* `Settings`

### Ermittelt die aktuelle API-Version. Pruft dabei, ob die angegebene API-Version noch verwendet werden kann

*Tags:* `Version`

#### Input Parameters
* `clientApiVersion` - _optional_ - API-Version, gegen die ein Client entwickelt wurde.

### Uberpruft eine der API bekannte Client-Version auf Aktualitat

*Tags:* `Version`

## License

**flow**ground :- Telekom iPaaS / xworks-api-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
