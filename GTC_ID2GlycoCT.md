# GlyTouCan

## 2019-10-03

* G57653LC のエントリーは、GlycoCTもWURCSもありません。

* SPARQL endpoint
 * https://endpoint.glycosmos.org/sparql

```
PREFIX glycan: <http://purl.jp/bio/12/glyco/glycan#>
PREFIX glytoucan:  <http://www.glytoucan.org/glyco/owl/glytoucan#>

SELECT DISTINCT ?PrimaryId ?Sequence
FROM <http://rdf.glytoucan.org/core>
FROM <http://rdf.glytoucan.org/sequence/glycoct>
WHERE {
    ?Saccharide glytoucan:has_primary_id ?PrimaryId .
    ?Saccharide glycan:has_glycosequence ?GlycoSequence .
    ?GlycoSequence glycan:has_sequence ?Sequence .
    ?GlycoSequence glycan:in_carbohydrate_format glycan:carbohydrate_format_glycoct.
    VALUES (?PrimaryId) { 
("G97036DW")
("G94712BS")
("G41353QW")
("G07602IS")
("G24976VE")
("G51798OK")
("G13459UO")
("G76430CU")
("G96656XQ")
("G53365WH")
("G23990FV")
("G79204BV")
("G98560IS")
("G24892LD")
("G52388NO")
("G42491HX")
("G38233WM")
("G62997JW")
("G24666QR")
("G19785QF")
("G80502ZO")
("G13545WA")
("G88544ZX")
("G88586UU")
("G09852PG")
("G88172YD")
("G07333YM")
("G51882YP")
("G38153WU")
("G01169LI")
("G23312HM")
("G82659EE")
("G98526YS")
("G20551IF")
("G64607RL")
("G83933JV")
("G55686UR")
("G43853TY")
("G32211HB")
("G45661AN")
("G85272PK")
("G10176IJ")
("G03392CR")
("G28767TB")
("G93422ES")
("G91479TJ")
("G40445KW")
("G57653LC")
("G67115BI")
("G89912DX")
("G75622JY")
("G43607XC")
("G65405NL")
("G51449DA")
("G53042AA")
("G60565BT")
("G98555FZ")
("G30930KH")
("G66797DB")
("G49108OO")
("G15170ZD")
("G92358QN")
("G29091VM")
("G91451DO")
("G55687NI")
("G70236BB")
("G12560BA")
("G60000IK")
("G51663TV")
("G02386YV")
("G31221HW")
("G82618CT")
("G34631OW")
("G56783UO")
("G66832EY")
("G86435AQ")
("G74275ML")
("G11569GN")
("G57243PH")
("G31381SZ")
("G34570EA")
("G27796KP")
("G58730ZZ")
("G85067IV")
("G21165PJ")
("G31648JS")
("G83816RY")
("G48931WX")
("G70709JG")
("G38540KX")
("G47580YI")
("G12286KP")
("G11035VI")
("G32728OO")
("G03045HJ")
("G12190WX")
("G12141RL")
("G15886VO")
("G55333QT")
("G01355BU")
("G09840KS")
("G78138NS")
("G75576ER")
("G80158KS")
("G35164EL")
("G37170NQ")
("G10244LO")
("G89318BF")
      }
}
ORDER BY ?PrimaryId
limit 200
```
