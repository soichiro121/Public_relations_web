# QRコードの形式の例
{ "qr_id": 5, "name": "講堂", "x": 560, "y": 160, "floor": 1}  
注意点として、{}で囲むのと、「,」で区切ること、""で囲むこと、間に「:」を入れることは忘れないでください。要は各部分の値だけ変えればいいってことです。
# x座標とy座標について
https://hayaoshi.com/bunkasai/getCoordinates.html から画像を選んで座標を取得してください。
# ここにいろんな場所のQRコードの文字を作成していってください。(画像は入れないでください。1つの場所につき1行でお願いします。)

# 経路について
      "A": { id: "A", name: "校門", x: 600, y: 125, floor: 1, neighbors: [ { id: "B", cost: 8 }, { id: "D", cost: 5 } ] },  
      "B": { id: "B", name: "廊下", x: 540, y: 125, floor: 1, neighbors: [ { id: "A", cost: 8 }, { id: "C", cost: 5 }, { id: "D", cost: 3 } ] },  
      "C": { id: "C", name: "講堂", x: 560, y: 160, floor: 1, neighbors: [ { id: "B", cost: 5 }, { id: "D", cost: 4 } ] },  
      "D": { id: "D", name: "A階段 (1F)", x: 796, y: 252, floor: 1, neighbors: [ { id: "B", cost: 3 }, { id: "C", cost: 4 }, { id: "E", cost: 5 } ] },  
      "E": { id: "E", name: "A階段 (2F)", x: 80, y: 120, floor: 2, neighbors: [ { id: "D", cost: 5 }, { id: "F", cost: 8 }, { id: "G", cost: 6 } ] },  
      "F": { id: "F", name: "食堂", x: 150, y: 200, floor: 1, neighbors: [ { id: "E", cost: 8 }, { id: "G", cost: 7 } ] },  
      "G": { id: "G", name: "音楽室", x: 180, y: 100, floor: 5, neighbors: [ { id: "E", cost: 6 }, { id: "F", cost: 7 } ] }  

      こんな感じでやってほしいんです。
# ここに経路を追加していってください。
      "A": { id: "A", name: "校門", x: 600, y: 125, floor: 1, neighbors: [ { id: "B", cost: 8 }, { id: "D", cost: 5 } ] },  
      "B": { id: "B", name: "廊下", x: 540, y: 125, floor: 1, neighbors: [ { id: "A", cost: 8 }, { id: "C", cost: 5 }, { id: "D", cost: 3 } ] },  
      "C": { id: "C", name: "講堂", x: 560, y: 160, floor: 1, neighbors: [ { id: "B", cost: 5 }, { id: "D", cost: 4 } ] },  
      "D": { id: "D", name: "A階段 (1F)", x: 796, y: 252, floor: 1, neighbors: [ { id: "B", cost: 3 }, { id: "C", cost: 4 }, { id: "E", cost: 5 } ] },  
      "E": { id: "E", name: "A階段 (2F)", x: 80, y: 120, floor: 2, neighbors: [ { id: "D", cost: 5 }, { id: "F", cost: 8 }, { id: "G", cost: 6 } ] },  
      "F": { id: "F", name: "食堂", x: 150, y: 200, floor: 1, neighbors: [ { id: "E", cost: 8 }, { id: "G", cost: 7 } ] },  
      "G": { id: "G", name: "音楽室", x: 180, y: 100, floor: 5, neighbors: [ { id: "E", cost: 6 }, { id: "F", cost: 7 } ] }   
