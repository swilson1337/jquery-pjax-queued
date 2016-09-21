Requires that you edit your web config and add the 'assetManager' component similar to this:

	'assetManager' => [
		'bundles' => [
			'yii\web\JqueryAsset' => [
				'jsOptions' => [
					'position' => \yii\web\View::POS_HEAD,
				],
			],
			'yii\widgets\PjaxAsset' => [
				'sourcePath' => '@vendor/swilson1337/jquery-pjax-queued',
				'js' => [
					'jquery.pjax.js',
				],
				'jsOptions' => [
					'position' => \yii\web\View::POS_HEAD,
				],
			],
		],
	],
