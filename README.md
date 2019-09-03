# jdatetimerich-ls
Formatting NotesDateTime as it is Java SimpleDateFormat

# Example how to use it
Private Function testJDTR
	Dim jdtr As New jDateTimeRich
	Dim dt As New NotesDateTime("15-10-2017 10:20:30")

	MsgBox jdtr.SimpleDateFormat(dt, "dd-MM-yyyy", "", "") ' "15-10-2017"
	MsgBox jdtr.SimpleDateFormat(dt, "d-MMM-yy", "ru", "RU") ' "15-окт-17"
	MsgBox jdtr.SimpleDateFormat(dt, "EEEEE MMMMM yyyy HH:mm:ss.SSSZ", "da", "DK") ' "søndag oktober 2017 11:20:30.000+0200")
End Function
