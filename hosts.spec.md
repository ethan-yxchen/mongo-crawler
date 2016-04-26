# BulletinBoard::hosts

*hosts* is a BulletinBoard (in implementation, a collection in a MongoDB database).

Each record in *hosts* represent one website. It is identified by the website's hostname, encoded with <a href="https://www.ietf.org/rfc/rfc3490.txt">IDNA</a>.

Required fields:
* status
  Current status of each host. Agents select valid target to perform actions, so this field 
  * IDLE
  * BUSY
  * WRONG
  * PAUSE
  * WAIT
