cmake_minimum_required(VERSION 3.3)
set(SOURCES
    iconv.c
    localcharset.c
    relocatable.c
)

set(HEADERS
    "../include/aliases.h"
    "../include/aliases_aix.h"
    "../include/aliases_aix_sysaix.h"
    "../include/aliases_dos.h"
    "../include/aliases_extra.h"
    "../include/aliases_osf1.h"
    "../include/aliases_osf1_sysosf1.h"
    "../include/aliases_sysaix.h"
    "../include/aliases_syshpux.h"
    "../include/aliases_sysosf1.h"
    "../include/aliases_syssolaris.h"
    "../include/aliases2.h"
    "../include/armscii_8.h"
    "../include/ascii.h"
    "../include/atarist.h"
    "../include/big5.h"
    "../include/big5_2003.h"
    "../include/big5hkscs1999.h"
    "../include/big5hkscs2001.h"
    "../include/big5hkscs2004.h"
    "../include/big5hkscs2008.h"
    "../include/c99.h"
    "../include/canonical.h"
    "../include/canonical_aix.h"
    "../include/canonical_aix_sysaix.h"
    "../include/canonical_dos.h"
    "../include/canonical_extra.h"
    "../include/canonical_local.h"
    "../include/canonical_local_sysaix.h"
    "../include/canonical_local_syshpux.h"
    "../include/canonical_local_sysosf1.h"
    "../include/canonical_local_syssolaris.h"
    "../include/canonical_osf1.h"
    "../include/canonical_osf1_sysosf1.h"
    "../include/canonical_sysaix.h"
    "../include/canonical_syshpux.h"
    "../include/canonical_sysosf1.h"
    "../include/canonical_syssolaris.h"
    "../include/ces_big5.h"
    "../include/ces_gbk.h"
    "../include/cjk_variants.h"
    "../include/cns11643.h"
    "../include/cns11643_1.h"
    "../include/cns11643_15.h"
    "../include/cns11643_2.h"
    "../include/cns11643_3.h"
    "../include/cns11643_4.h"
    "../include/cns11643_4a.h"
    "../include/cns11643_4b.h"
    "../include/cns11643_5.h"
    "../include/cns11643_6.h"
    "../include/cns11643_7.h"
    "../include/cns11643_inv.h"
    "../include/config.h"
    "../include/converters.h"
    "../include/cp1046.h"
    "../include/cp1124.h"
    "../include/cp1125.h"
    "../include/cp1129.h"
    "../include/cp1131.h"
    "../include/cp1133.h"
    "../include/cp1161.h"
    "../include/cp1162.h"
    "../include/cp1163.h"
    "../include/cp1250.h"
    "../include/cp1251.h"
    "../include/cp1252.h"
    "../include/cp1253.h"
    "../include/cp1254.h"
    "../include/cp1255.h"
    "../include/cp1256.h"
    "../include/cp1257.h"
    "../include/cp1258.h"
    "../include/cp437.h"
    "../include/cp737.h"
    "../include/cp775.h"
    "../include/cp850.h"
    "../include/cp852.h"
    "../include/cp853.h"
    "../include/cp855.h"
    "../include/cp856.h"
    "../include/cp857.h"
    "../include/cp858.h"
    "../include/cp860.h"
    "../include/cp861.h"
    "../include/cp862.h"
    "../include/cp863.h"
    "../include/cp864.h"
    "../include/cp865.h"
    "../include/cp866.h"
    "../include/cp869.h"
    "../include/cp874.h"
    "../include/cp922.h"
    "../include/cp932.h"
    "../include/cp932ext.h"
    "../include/cp936.h"
    "../include/cp936ext.h"
    "../include/cp943.h"
    "../include/cp949.h"
    "../include/cp950.h"
    "../include/cp950ext.h"
    "../include/dec_hanyu.h"
    "../include/dec_kanji.h"
    "../include/encodings.def"
    "../include/encodings_aix.def"
    "../include/encodings_dos.def"
    "../include/encodings_extra.def"
    "../include/encodings_local.def"
    "../include/encodings_osf1.def"
    "../include/euc_cn.h"
    "../include/euc_jisx0213.h"
    "../include/euc_jp.h"
    "../include/euc_kr.h"
    "../include/euc_tw.h"
    "../include/flags.h"
    "../include/flushwc.h"
    "../include/gb12345.h"
    "../include/gb12345ext.h"
    "../include/gb18030.h"
    "../include/gb18030ext.h"
    "../include/gb18030uni.h"
    "../include/gb2312.h"
    "../include/gbk.h"
    "../include/gbkext_inv.h"
    "../include/gbkext1.h"
    "../include/gbkext2.h"
    "../include/georgian_academy.h"
    "../include/georgian_ps.h"
    "../include/hkscs1999.h"
    "../include/hkscs2001.h"
    "../include/hkscs2004.h"
    "../include/hkscs2008.h"
    "../include/hp_roman8.h"
    "../include/hz.h"
    "../include/iconv.h"
    "../include/iconv_open1.h"
    "../include/iconv_open2.h"
    "../include/iso2022_cn.h"
    "../include/iso2022_cnext.h"
    "../include/iso2022_jp.h"
    "../include/iso2022_jp1.h"
    "../include/iso2022_jp2.h"
    "../include/iso2022_jp3.h"
    "../include/iso2022_kr.h"
    "../include/iso646_cn.h"
    "../include/iso646_jp.h"
    "../include/iso8859_1.h"
    "../include/iso8859_10.h"
    "../include/iso8859_11.h"
    "../include/iso8859_13.h"
    "../include/iso8859_14.h"
    "../include/iso8859_15.h"
    "../include/iso8859_16.h"
    "../include/iso8859_2.h"
    "../include/iso8859_3.h"
    "../include/iso8859_4.h"
    "../include/iso8859_5.h"
    "../include/iso8859_6.h"
    "../include/iso8859_7.h"
    "../include/iso8859_8.h"
    "../include/iso8859_9.h"
    "../include/isoir165.h"
    "../include/isoir165ext.h"
    "../include/java.h"
    "../include/jisx0201.h"
    "../include/jisx0208.h"
    "../include/jisx0212.h"
    "../include/jisx0213.h"
    "../include/johab.h"
    "../include/johab_hangul.h"
    "../include/koi8_r.h"
    "../include/koi8_ru.h"
    "../include/koi8_t.h"
    "../include/koi8_u.h"
    "../include/ksc5601.h"
    "../include/loop_unicode.h"
    "../include/loop_wchar.h"
    "../include/loops.h"
    "../include/mac_arabic.h"
    "../include/mac_centraleurope.h"
    "../include/mac_croatian.h"
    "../include/mac_cyrillic.h"
    "../include/mac_greek.h"
    "../include/mac_hebrew.h"
    "../include/mac_iceland.h"
    "../include/mac_roman.h"
    "../include/mac_romania.h"
    "../include/mac_thai.h"
    "../include/mac_turkish.h"
    "../include/mac_ukraine.h"
    "../include/mulelao.h"
    "../include/nextstep.h"
    "../include/pt154.h"
    "../include/relocatable.h"
    "../include/riscos1.h"
    "../include/rk1048.h"
    "../include/shift_jisx0213.h"
    "../include/sjis.h"
    "../include/tcvn.h"
    "../include/tds565.h"
    "../include/tis620.h"
    "../include/translit.def"
    "../include/translit.h"
    "../include/ucs2.h"
    "../include/ucs2be.h"
    "../include/ucs2internal.h"
    "../include/ucs2le.h"
    "../include/ucs2swapped.h"
    "../include/ucs4.h"
    "../include/ucs4be.h"
    "../include/ucs4internal.h"
    "../include/ucs4le.h"
    "../include/ucs4swapped.h"
    "../include/uhc_1.h"
    "../include/uhc_2.h"
    "../include/utf16.h"
    "../include/utf16be.h"
    "../include/utf16le.h"
    "../include/utf32.h"
    "../include/utf32be.h"
    "../include/utf32le.h"
    "../include/utf7.h"
    "../include/utf8.h"
    "../include/vietcomb.h"
    "../include/viscii.h"
)

add_library(${LIOCONV} STATIC ${SOURCES} ${HEADERS})
