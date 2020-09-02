# mahonia
Mahonia—a character-set conversion library for Go

Mahonia is a character-set conversion library implemented in Go. All data is compiled into the executable; it doesn't need any external data files.

Mahonia is now deprecated. I recommend using the standard package at golang.org/x/text/encoding, possibly along with golang.org/x/net/charset

 based on http://code.google.com/p/mahonia/

install
-------

	go get github.com/gaogaogoo/mahonia

example
-------

	package main
	import "fmt"
	import "github.com/gaogaogoo/mahonia"
	func main(){
	  enc:=mahonia.NewEncoder("gbk")
	  //converts a  string from UTF-8 to gbk encoding.
	  fmt.Println(enc.ConvertString("hello,世界"))  
	
