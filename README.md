# XMLSimple
1.
    На основании запроса
    SELECT ID_ART,NAME,CODE,USERNAME,GUID FROM WHS.ARTICLE where rownum < 10000
    Сформировать XML вида :
        <articles>
            <articles id_art="104880" name="Батон нарезной в/с 0.4кг" code="1010050114" username="WHS" guid="6992B998083711DC87F900093D12899D">
        ...
        </articles>
    
2.
    Написать XSLT преобразование, которое приведет xml, полученный в предыдущей задаче к виду:
<articles>
    <article>
        <id_art>104880</id_art>
        <name>Батон нарезной в/с 0.4кг</name>
        <code>1010050114</code>
        <username>WHS</username>
        <guid>6992B998083711DC87F900093D12899D</guid>
    </article>
    ...
</articles>
Применять преобразование можно в Eclipse, предварительно сконфигурировав XSLT процессор SAXON.
