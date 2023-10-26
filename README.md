# JQueryNiceSelect


```js
// select Box 처리
export const initSelectBoxUI = (list) => {
    list.length !== 0 && list.map(data => {
        $(data.className).val();
        $(data.className).off("change").on("change", data.handleFunction);
    })
}


export const choiceSelectBoxUI = (data) => {
    $(data.className).val(data.value);
    $(data.className).niceSelect('update');
}

```


JQuery 사용했을 때 나이스셀렉트로 퍼블리싱을 받아서 고생했었는데 NiceSelect 기본 구성 메소드를 정리해두었습니다.
