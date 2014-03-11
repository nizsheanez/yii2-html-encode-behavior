Automatic Html::encode/Html::decode when you save/find model

###Usage

1) Install with Composer

~~~php

"require": {
    "nizsheanez/yii2-html-encode-behavior": "1.*",
},

php composer.phar update

~~~php
public function behaviors()
{
    return ArrayHelper::merge(parent::behaviors(), [
        'htmlEncode' => [
            'class'      => 'common\components\behaviors\HtmlEncode',
            'attributes' => [
                'description',
                'someAttributeForWysiwyg',
            ],
        ],
    ]);
}
~~~






