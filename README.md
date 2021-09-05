# CSS Flexbox
### CSS Flexbox လမ်းညွှန်
ဒီ CSS Flexbox လမ်းညွှန်မှာ CSS ရဲ့ Flex Container, Flex Items, သူတို့ရဲ့ Properties & Values, သူတို့အလုပ်လုပ်ပုံတွေကို လေ့လာနိုင်ပါတယ်။

#### Flex Container
- [flex-direction](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#flex-direction-container)
- [flex-wrap](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#flex-wrap-container)
- [flex-flow](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#flex-flow-container)
- [justify-content](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#justify-content-container)
- [align-items](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#align-items-container)
- [align-content](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#align-content-container)

#### Flex Items
- [order](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#order-items)
- [flex-grow](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#flex-grow-items)
- [flex-shrink](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#flex-shrink-items)
- [flex-basis](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#flex-basis-items)
- [flex](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#flex-items-1)
- [align-self](https://github.com/mrminnkhantnaing/css-flexbox/new/main?readme=1#align-self-items)

---

#### flex-direction (Container)
- column
- column-reverse
- row
- row-reverse

#### flex-wrap (Container)
- wrap
- nowrap
- wrap-reverse

#### flex-flow (Container)
- row wrap
- row nowrap
- row wrap-reverse

#### justify-content (Container)
- center
- flex-start
- flex-end
- space-around
- space-between
- space-evenly

#### align-items (Container)
- center
- flex-start
- flex-end
- stretch
- baseline

#### align-content (Container)
- center
- flex-start
- flex-end
- space-around
- space-between
- space-evenly

---

#### order (Items)
- 'order' property ကို flex items တွေရဲ့ အစီအစဉ်ကို ပြောင်းလဲဖို့ အသုံးပြုနိုင်ပါတယ်။
- 'order' ရဲ့ value ဟာ နံပါတ်ပဲ ဖြစ်ရပါမယ်။ မူလတန်ဖိုးကို '0' လို့ သတ်မှတ်ထားပါတယ်။
```
<div class="flex-container">
  <div style="order: 3;">1</div>
  <div style="order: 2;">2</div>
  <div style="order: 4;">3</div>
  <div style="order: 1;">4</div>
</div>
```

#### flex-grow (Items)
- 'flex-grow' ကို 'flex item' ရဲ့ အကြီးဆုံးဖြစ်လာမယ့် အရွယ်အစားကို သတ်မှတ်တဲ့အခါ အသုံးပြုပါတယ်။
- 'flex-grow' ရဲ့ value ဟာ နံပါတ်ပဲ ဖြစ်ရပါမယ်။ မူလတန်ဖိုးကို '0' လို့ သတ်မှတ်ထားပါတယ်။
```
<div class="flex-container">
  <div style="flex-grow: 1;">1</div>
  <div style="flex-grow: 1;">2</div>
  <div style="flex-grow: 8;">3</div>
</div>
```

#### flex-shrink (Items)
- 'flex-shrink' ကို 'flex item' ရဲ့ အငယ်ဆုံးဖြစ်လာမယ့် အရွယ်အစားကို သတ်မှတ်တဲ့အခါ အသုံးပြုပါတယ်။
- 'flex-shrink' ရဲ့ value ဟာ နံပါတ်ပဲ ဖြစ်ရပါမယ်။ မူလတန်ဖိုးကို '0' လို့ သတ်မှတ်ထားပါတယ်။
```
<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div style="flex-shrink: 0;">3</div>
  <div>4</div>
</div>
```

#### flex-basis (Items)
- 'flex-basis' property ကို နဂိုရှိနေမယ့် 'flex item' ရဲ့ အရွယ်အစားကို သတ်မှတ်တဲ့အခါ အသုံးပြုနိုင်ပါတယ်။
```
<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div style="flex-basis: 200px;">3</div>
  <div>4</div>
</div>
```

#### flex (Items)
- 'flex' property ဟာ flex-grow, flex-shrink နှင့် flex-basis properties (၃) ခုစလုံးကို တစ်နေရာတည်းမှာ ကြေညာနိုင်တဲ့ Shorthand ဖြစ်ပါတယ်။
```
<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div style="flex: 0 0 200px;">3</div>
  <div>4</div>
</div>
```

#### align-self (Items)
- 'align-self' property ဟာ flexible container ထဲက ရွေးချယ်ထားတဲ့ item တစ်ခုတည်းရဲ့ alignment ကို သတ်မှတ်တဲ့အခါ အသုံးပြုပါတယ်။
- 'align-self' property ဟာ flex container ရဲ့ align-items property မှာ သတ်မှတ်ထားတဲ့ တန်ဖိုးကို override လုပ်ပြီး သူ့တန်ဖိုးကိုပဲ အသုံးပြုပါတယ်။
```
<div class="flex-container">
  <div>1</div>
  <div style="align-self: flex-start;">2</div>
  <div style="align-self: flex-end";>3</div>
  <div>4</div>
</div>
```

The end of this short guide...
