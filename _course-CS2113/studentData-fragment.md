{% set tutorials = [

]%}

{% set students = [

]%}

{% set teams = {

}%}

{% set products = {

}%}

{% set users = {

}%}

{% set values = {

}%}

{# format: [team, reviewer, reviewee1, backup1, reviewee2, backup2]
From the same tutorial. One for coding standard review, one for code quality.
 #}

{% set ip_pr_review_allocation = [
['CS2113-F11', 'Cheezeblokz', 'kaijie0102', 'StanleyW00', 'J-Y-Yan', 'Cheezeblokz'],
['CS2113-F11', 'kaijie0102', 'StanleyW00', 'J-Y-Yan', 'Cheezeblokz', 'kaijie0102'],
['CS2113-F11', 'charkty', 'wendelinwemhoener', 'MrOPPA1', 'kevinz420', 'charkty'],
['CS2113-F11', 'StanleyW00', 'J-Y-Yan', 'Cheezeblokz', 'kaijie0102', 'StanleyW00'],
['CS2113-F11', 'wendelinwemhoener', 'MrOPPA1', 'kevinz420', 'charkty', 'wendelinwemhoener'],
['CS2113-F11', 'J-Y-Yan', 'Cheezeblokz', 'kaijie0102', 'StanleyW00', 'J-Y-Yan'],
['CS2113-F11', 'kevinz420', 'charkty', 'wendelinwemhoener', 'MrOPPA1', 'kevinz420'],
['CS2113-F11', 'MrOPPA1', 'kevinz420', 'charkty', 'wendelinwemhoener', 'MrOPPA1'],
['CS2113-F11', 'junhyeong0411', 'Remy9926', 'Brian030601', 'Haoyuli2002', 'junhyeong0411'],
['CS2113-F11', 'Haoyuli2002', 'junhyeong0411', 'Remy9926', 'Brian030601', 'Haoyuli2002'],
['CS2113-F11', 'Remy9926', 'Brian030601', 'Haoyuli2002', 'junhyeong0411', 'Remy9926'],
['CS2113-F11', 'Brian030601', 'Haoyuli2002', 'junhyeong0411', 'Remy9926', 'Brian030601'],
['CS2113-T17', 'aaronxujiachen', 'onx001', 'rohitcube', 'YFshadaow', 'ziyi105'],
['CS2113-T17', 'yicheng-toh', 'TeoHaoZhi', 'limyuhching', 'Barbaracwx', 'ShaniceTang'],
['CS2113-T17', 'nihalzp', 'DaDevChia', 'lckjosh', 'vvhuiling', 'spaceman03'],
['CS2113-T17', 'bljhty', 'TongZhengHong', 'janelleenqi', 'NaychiMin', 'ryanlohyr'],
['CS2113-T17', 'Zhang-Zhitong', 'azfarulmatin', 'martinschnder', 'AlWo223', 'skylee03'],
['CS2113-T17', 'limyuhching', 'Barbaracwx', 'ShaniceTang', 'NeoMinWei', 'karishma-t'],
['CS2113-T17', 'DextheChik3n', 'yicheng-toh', 'TeoHaoZhi', 'limyuhching', 'Barbaracwx'],
['CS2113-T17', 'ziyi105', 'ryan1604', 'choonkit-nus', 'KenCheung18', 'ken-ruster'],
['CS2113-T17', 'onx001', 'rohitcube', 'YFshadaow', 'ziyi105', 'ryan1604'],
['CS2113-T17', 'TongZhengHong', 'janelleenqi', 'NaychiMin', 'ryanlohyr', 'Zhang-Zhitong'],
['CS2113-T17', 'ken-ruster', 'nihalzp', 'DaDevChia', 'lckjosh', 'vvhuiling'],
['CS2113-T17', 'TeoHaoZhi', 'limyuhching', 'Barbaracwx', 'ShaniceTang', 'NeoMinWei'],
['CS2113-T17', 'NeoMinWei', 'karishma-t', 'Cazh1', 'TriciaBK', 'aaronxujiachen'],
['CS2113-T17', 'wwweert123', 'hshiah', 'antrikshdhand', 'SebasFok', 'bljhty'],
['CS2113-T17', 'SebasFok', 'bljhty', 'TongZhengHong', 'janelleenqi', 'NaychiMin'],
['CS2113-T17', 'DaDevChia', 'lckjosh', 'vvhuiling', 'spaceman03', 'wwweert123'],
['CS2113-T17', 'Cazh1', 'TriciaBK', 'aaronxujiachen', 'onx001', 'rohitcube'],
['CS2113-T17', 'ryan1604', 'choonkit-nus', 'KenCheung18', 'ken-ruster', 'nihalzp'],
['CS2113-T17', 'azfarulmatin', 'martinschnder', 'AlWo223', 'skylee03', 'Hongzhii'],
['CS2113-T17', 'ShaniceTang', 'NeoMinWei', 'karishma-t', 'Cazh1', 'TriciaBK'],
['CS2113-T17', 'NaychiMin', 'ryanlohyr', 'Zhang-Zhitong', 'azfarulmatin', 'martinschnder'],
['CS2113-T17', 'rohitcube', 'YFshadaow', 'ziyi105', 'ryan1604', 'choonkit-nus'],
['CS2113-T17', 'janelleenqi', 'NaychiMin', 'ryanlohyr', 'Zhang-Zhitong', 'azfarulmatin'],
['CS2113-T17', 'YFshadaow', 'ziyi105', 'ryan1604', 'choonkit-nus', 'KenCheung18'],
['CS2113-T17', 'ryanlohyr', 'Zhang-Zhitong', 'azfarulmatin', 'martinschnder', 'AlWo223'],
['CS2113-T17', 'Barbaracwx', 'ShaniceTang', 'NeoMinWei', 'karishma-t', 'Cazh1'],
['CS2113-T17', 'karishma-t', 'Cazh1', 'TriciaBK', 'aaronxujiachen', 'onx001'],
['CS2113-T17', 'TriciaBK', 'aaronxujiachen', 'onx001', 'rohitcube', 'YFshadaow'],
['CS2113-T17', 'lckjosh', 'vvhuiling', 'spaceman03', 'wwweert123', 'hshiah'],
['CS2113-T17', 'Hongzhii', 'CerIsaiah', 'DextheChik3n', 'yicheng-toh', 'TeoHaoZhi'],
['CS2113-T17', 'AlWo223', 'skylee03', 'Hongzhii', 'CerIsaiah', 'DextheChik3n'],
['CS2113-T17', 'KenCheung18', 'ken-ruster', 'nihalzp', 'DaDevChia', 'lckjosh'],
['CS2113-T17', 'skylee03', 'Hongzhii', 'CerIsaiah', 'DextheChik3n', 'yicheng-toh'],
['CS2113-T17', 'spaceman03', 'wwweert123', 'hshiah', 'antrikshdhand', 'SebasFok'],
['CS2113-T17', 'hshiah', 'antrikshdhand', 'SebasFok', 'bljhty', 'TongZhengHong'],
['CS2113-T17', 'antrikshdhand', 'SebasFok', 'bljhty', 'TongZhengHong', 'janelleenqi'],
['CS2113-T17', 'vvhuiling', 'spaceman03', 'wwweert123', 'hshiah', 'antrikshdhand'],
['CS2113-T17', 'martinschnder', 'AlWo223', 'skylee03', 'Hongzhii', 'CerIsaiah'],
['CS2113-T17', 'CerIsaiah', 'DextheChik3n', 'yicheng-toh', 'TeoHaoZhi', 'limyuhching'],
['CS2113-T17', 'choonkit-nus', 'KenCheung18', 'ken-ruster', 'nihalzp', 'DaDevChia'],
['CS2113-W12', 'sRanay', 'tangzhenen', 'farissirraj', 'bnjm2000', 'ChoonSiang'],
['CS2113-W12', 'mcmc101001', 'yeo-menghan', 'DavinciDelta', 'yingx9', 'J0shuaLeong'],
['CS2113-W12', 'NgLixuanNixon', 'WooKaiNing', 'Xuan127', 'itayrefaely', 'hooami'],
['CS2113-W12', 'farissirraj', 'bnjm2000', 'ChoonSiang', 'spinoandraptos', 'imaginarys96'],
['CS2113-W12', 'StevenGX12', '000verflow', 'sRanay', 'tangzhenen', 'farissirraj'],
['CS2113-W12', 'BenedictChannn', 'ICubE-', 'lctxct', 'JoanneJo', 'woodenclock'],
['CS2113-W12', 'yeo-menghan', 'DavinciDelta', 'yingx9', 'J0shuaLeong', 'Jonoans'],
['CS2113-W12', 'Jonoans', 'BenedictChannn', 'ICubE-', 'lctxct', 'JoanneJo'],
['CS2113-W12', 'ChoonSiang', 'spinoandraptos', 'imaginarys96', 'James-Hong-Jey', 'lisizhuang-0121'],
['CS2113-W12', 'J0shuaLeong', 'Jonoans', 'BenedictChannn', 'ICubE-', 'lctxct'],
['CS2113-W12', 'James-Hong-Jey', 'lisizhuang-0121', 'danielpappa', 'mcmc101001', 'yeo-menghan'],
['CS2113-W12', 'WooKaiNing', 'Xuan127', 'itayrefaely', 'hooami', 'StevenGX12'],
['CS2113-W12', 'spinoandraptos', 'imaginarys96', 'James-Hong-Jey', 'lisizhuang-0121', 'danielpappa'],
['CS2113-W12', 'Xuan127', 'itayrefaely', 'hooami', 'StevenGX12', '000verflow'],
['CS2113-W12', 'hooami', 'StevenGX12', '000verflow', 'sRanay', 'tangzhenen'],
['CS2113-W12', 'danielpappa', 'mcmc101001', 'yeo-menghan', 'DavinciDelta', 'yingx9'],
['CS2113-W12', 'ICubE-', 'lctxct', 'JoanneJo', 'woodenclock', 'marklin2234'],
['CS2113-W12', 'marklin2234', 'NgLixuanNixon', 'WooKaiNing', 'Xuan127', 'itayrefaely'],
['CS2113-W12', 'itayrefaely', 'hooami', 'StevenGX12', '000verflow', 'sRanay'],
['CS2113-W12', 'lisizhuang-0121', 'danielpappa', 'mcmc101001', 'yeo-menghan', 'DavinciDelta'],
['CS2113T-W11', 'woodenclock', 'marklin2234', 'NgLixuanNixon', 'WooKaiNing', 'Xuan127'],
['CS2113T-W11', 'tangzhenen', 'farissirraj', 'bnjm2000', 'ChoonSiang', 'spinoandraptos'],
['CS2113T-W11', 'imaginarys96', 'James-Hong-Jey', 'lisizhuang-0121', 'danielpappa', 'mcmc101001'],
['CS2113T-W11', 'lctxct', 'JoanneJo', 'woodenclock', 'marklin2234', 'NgLixuanNixon'],
['CS2113T-W11', 'bnjm2000', 'ChoonSiang', 'spinoandraptos', 'imaginarys96', 'James-Hong-Jey'],
['CS2113T-W11', 'DavinciDelta', 'yingx9', 'J0shuaLeong', 'Jonoans', 'BenedictChannn'],
['CS2113T-W11', 'yingx9', 'J0shuaLeong', 'Jonoans', 'BenedictChannn', 'ICubE-'],
['CS2113T-W11', 'JoanneJo', 'woodenclock', 'marklin2234', 'NgLixuanNixon', 'WooKaiNing'],
['CS2113T-W11', '000verflow', 'sRanay', 'tangzhenen', 'farissirraj', 'bnjm2000']
]%}

{% set ip_pr_slap_review_allocation = [
['000verflow', 'ziyi105', 'TriciaBK'],
['AlWo223', 'James-Hong-Jey', 'kaijie0102'],
['Barbaracwx', 'BenedictChannn', 'DavinciDelta'],
['BenedictChannn', 'DavinciDelta', 'Zhang-Zhitong'],
['Brian030601', 'ShaniceTang', 'choonkit-nus'],
['Cazh1', 'vvhuiling', 'ICubE-'],
['CerIsaiah', 'itayrefaely', 'Haoyuli2002'],
['Cheezeblokz', 'onx001', 'lckjosh'],
['ChoonSiang', '000verflow', 'ziyi105'],
['DaDevChia', 'antrikshdhand', 'danielpappa'],
['DavinciDelta', 'Zhang-Zhitong', 'ryanlohyr'],
['DextheChik3n', 'karishma-t', 'yeo-menghan'],
['Haoyuli2002', 'ryan1604', 'martinschnder'],
['Hongzhii', 'J0shuaLeong', 'Cheezeblokz'],
['ICubE-', 'MrOPPA1', 'DaDevChia'],
['J-Y-Yan', 'wwweert123', 'spaceman03'],
['J0shuaLeong', 'Cheezeblokz', 'onx001'],
['James-Hong-Jey', 'kaijie0102', 'TongZhengHong'],
['JoanneJo', 'DextheChik3n', 'karishma-t'],
['Jonoans', 'JoanneJo', 'DextheChik3n'],
['KenCheung18', 'WooKaiNing', 'charkty'],
['MrOPPA1', 'DaDevChia', 'antrikshdhand'],
['NaychiMin', 'sRanay', 'woodenclock'],
['NeoMinWei', 'skylee03', 'spinoandraptos'],
['NgLixuanNixon', 'imaginarys96', 'yicheng-toh'],
['Remy9926', 'azfarulmatin', 'CerIsaiah'],
['SebasFok', 'hshiah', 'hooami'],
['ShaniceTang', 'choonkit-nus', 'lisizhuang-0121'],
['StanleyW00', 'TeoHaoZhi', 'KenCheung18'],
['StevenGX12', 'bnjm2000', 'bljhty'],
['TeoHaoZhi', 'KenCheung18', 'WooKaiNing'],
['TongZhengHong', 'Hongzhii', 'J0shuaLeong'],
['TriciaBK', 'Jonoans', 'JoanneJo'],
['WooKaiNing', 'charkty', 'ken-ruster'],
['Xuan127', 'wendelinwemhoener', 'NeoMinWei'],
['YFshadaow', 'farissirraj', 'lctxct'],
['Zhang-Zhitong', 'ryanlohyr', 'StevenGX12'],
['aaronxujiachen', 'NaychiMin', 'sRanay'],
['antrikshdhand', 'danielpappa', 'kevinz420'],
['azfarulmatin', 'CerIsaiah', 'itayrefaely'],
['bljhty', 'YFshadaow', 'farissirraj'],
['bnjm2000', 'bljhty', 'YFshadaow'],
['charkty', 'ken-ruster', 'AlWo223'],
['danielpappa', 'kevinz420', 'SebasFok'],
['farissirraj', 'lctxct', 'nihalzp'],
['hooami', 'J-Y-Yan', 'wwweert123'],
['hshiah', 'hooami', 'J-Y-Yan'],
['imaginarys96', 'yicheng-toh', 'rohitcube'],
['itayrefaely', 'Haoyuli2002', 'ryan1604'],
['janelleenqi', 'NgLixuanNixon', 'imaginarys96'],
['junhyeong0411', 'Cazh1', 'vvhuiling'],
['kaijie0102', 'TongZhengHong', 'Hongzhii'],
['karishma-t', 'yeo-menghan', 'yingx9'],
['ken-ruster', 'AlWo223', 'James-Hong-Jey'],
['kevinz420', 'SebasFok', 'hshiah'],
['lckjosh', 'ChoonSiang', '000verflow'],
['lctxct', 'nihalzp', 'janelleenqi'],
['limyuhching', 'Barbaracwx', 'BenedictChannn'],
['lisizhuang-0121', 'Remy9926', 'azfarulmatin'],
['marklin2234', 'junhyeong0411', 'Cazh1'],
['martinschnder', 'marklin2234', 'junhyeong0411'],
['mcmc101001', 'tangzhenen', 'aaronxujiachen'],
['nihalzp', 'janelleenqi', 'NgLixuanNixon'],
['onx001', 'lckjosh', 'ChoonSiang'],
['rohitcube', 'mcmc101001', 'tangzhenen'],
['ryan1604', 'martinschnder', 'marklin2234'],
['ryanlohyr', 'StevenGX12', 'bnjm2000'],
['sRanay', 'woodenclock', 'Brian030601'],
['skylee03', 'spinoandraptos', 'StanleyW00'],
['spaceman03', 'Xuan127', 'wendelinwemhoener'],
['spinoandraptos', 'StanleyW00', 'TeoHaoZhi'],
['tangzhenen', 'aaronxujiachen', 'NaychiMin'],
['choonkit-nus', 'lisizhuang-0121', 'Remy9926'],
['vvhuiling', 'ICubE-', 'MrOPPA1'],
['wendelinwemhoener', 'NeoMinWei', 'skylee03'],
['woodenclock', 'Brian030601', 'ShaniceTang'],
['wwweert123', 'spaceman03', 'Xuan127'],
['yeo-menghan', 'yingx9', 'limyuhching'],
['yicheng-toh', 'rohitcube', 'mcmc101001'],
['yingx9', 'limyuhching', 'Barbaracwx'],
['ziyi105', 'TriciaBK', 'Jonoans']
]%}

{% set tp_dg_review_allocation = [

] %}

{% set team_review_allocation = [

] %}
