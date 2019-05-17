function replaceAll(str, find, replace) {
    return str.replace(new RegExp(find, 'g'), replace);
}

function dec2hex(dec, padding){
  return parseInt(dec, 10).toString(16).padStart(padding, '0');
}

function utf8StringToUtf16String(str) {
  var utf16 = [];
  for (var i=0, strLen=str.length; i < strLen; i++) {
    utf16.push('\\\\u')
    utf16.push(dec2hex(str.charCodeAt(i), 4));
  }
  return utf16.join('');
}


var keywords = ['临冬城', '君临城', '提利昂', '兰尼斯特', '詹姆', '小恶魔', '弑君者', '瑟曦', '丹妮莉丝', '坦格利安', '龙之母', '龙母', '龙妈', '琼恩', '雪诺', '白狼主', '珊莎', '史塔克', '艾莉亚', '席恩', '布兰', '猎犬', '桑铎', '克里冈', '瓦里斯', '八爪蜘蛛', '老熊', '小熊女', '梅丽珊卓', '红袍女巫', '戴佛斯', '洋葱骑士', '三傻', '二丫', '夜王', '异鬼', '美人', '灰虫子', '熊岛', '艾丽娅', '私生子', '佛雷', '光之王', '莱安娜', '地窖', '骑士', '洋葱骑士', '奈德', '布蕾妮', '艾迪', '大熊', '山姆', '弥桑黛'];

var result = body;

keywords.forEach(function(k) {
  result = replaceAll(result, k, '喵喵喵');
  result = replaceAll(result, utf8StringToUtf16String(k), "\u55b5\u55b5\u55b5");  
});

result;
