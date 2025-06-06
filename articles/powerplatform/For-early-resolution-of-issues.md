---
title: Dynamics 365 Customer Engagement サポートチームより問題の早期解決に向けたお客様へのお願い
date: 2022-11-28 09:00:00
tags:
  - Dynamics
  - Dynamics 365
  - お問い合わせ全般
categories:
  - [Dynamics 365]
---

# Dynamics 365 Customer Engagement サポートチームより問題の早期解決に向けたお客様へのお願い

こんにちは、Power Platform サポートチームの鎌田です。

いつも Dynamics 365 をご利用いただきありがとうございます。
本記事では、Dynamics 365 をご利用されている皆様へ、問題の早期解決のためにサポートチームからお客様へのお願いを申し上げます。
ぜひお問い合わせの際にご確認をいただけますと幸いです。

## 目次

- [Dynamics 365 Customer Engagement サポートチームより問題の早期解決に向けたお客様へのお願い](#dynamics-365-customer-engagement-サポートチームより問題の早期解決に向けたお客様へのお願い)
  - [目次](#目次)
  - [調査のための情報ご提供のお願い](#調査のための情報ご提供のお願い)
  - [問題の正確な理解](#問題の正確な理解)
  - [切り分け情報](#切り分け情報)
  - [業務影響、達成事項、背景やスケジュール](#業務影響達成事項背景やスケジュール)
  - [サポート インスタンスについて](#サポート-インスタンスについて)
  - [仕様の確認に関する調査について](#仕様の確認に関する調査について)
  - [カスタマイズにより問題が発生している場合](#カスタマイズにより問題が発生している場合)
  - [参考](#参考)

## 調査のための情報ご提供のお願い

問題の調査を進めるために、お客様に問題を特定するための情報および問題の再現手順のご提供をお願いしております。後述の情報をお問い合わせ時にご提供いただけますとスムーズに調査を開始可能です。
調査に必要な情報が不足する場合は、調査が難航したり、解決が難しくなるケースがあり、調査に必要な情報をご提供いただけるまで、ご対応を一旦終了とさせていただくことがございます。

また、データセンター内の更新頻度が高いため、調査には最新の情報を必要とします。そのため、ご提供頂きました情報が古い場合、調査が困難になる場合があり、同じ情報のご提供を複数回お願いさせていただくことがございます。
何卒、お客様のご理解、ご協力のほどお願い申し上げます。

## 問題の正確な理解

発生事象の正確な把握が問題解決の第一歩となります。正確な情報をご提供いただき事象が具体的になれば、サポート エンジニアはより具体的に調査観点の絞り込みができます。弊社にて事象を再現させることができれば、より迅速な調査が可能となります。

下記にご提供いただきたい情報の例をご紹介いたします。なお、再現手順を文章で具体的に記載いただくことや、事象発生時の画面のキャプチャは発生事象の把握に非常に有用です。発生事象に対するお客様とエンジニアの認識が一致するようにご提供いただけますと幸いです。

- 事象発生日時（例：MM 月 DD 日 午前 HH 時 MM 分頃。分単位はおおよそでも問題ございません）
- 事象発生ユーザーの UPN
- 事象発生環境 URL
- 事象発生が確認できる画面キャプチャ
- エラーメッセージをコピーしたテキストファイル
- 事象発生時の操作内容や再現手順
- 再現時のビデオや、[問題ステップ レコーダー (PSR)](https://learn.microsoft.com/ja-jp/office/troubleshoot/settings/how-to-use-problem-steps-recorder) ログ

また、事象再現時のクライアントとサーバー間の通信を確認するために下記ログの採取をご依頼する場合がございます。事象再現時時の RequestID や正確な日時がわかるため、エラーだけでなく、サーバーからの応答遅延などの問題にも素早く正確な調査を開始できます。

- [Fiddler](https://social.technet.microsoft.com/Forums/azure/ja-JP/fe5f977a-2992-44c3-b643-38ad570a3d18/fiddler-12525124641239825505214622516338918?forum=DCRMSupport)
- [ブラウザ トレース ログ](https://learn.microsoft.com/ja-jp/azure/azure-portal/capture-browser-trace#google-chrome-and-microsoft-edge)
※上記リンクの手順にて、「Azure Portal」は、事象が発生する Dynamics 365 / Power Platform のアドレスへ読み替えてください。

オンプレミス版の Dynamics をご利用いただいている場合、下記情報もご共有くださいますと幸いです。

- ネットワーク図
- Dynamics 365 Server version
- SQL Server Edition / version
- Windows Server OS Edition / version

## 切り分け情報

問題の切り分けが可能であれば、切り分け結果をご共有ください。何を切り分けするかは事象によりケース バイ ケースですが、一般的な切り分け例をご紹介いたします。

- [ブラウザのキャッシュ クリア](https://support.microsoft.com/ja-jp/microsoft-edge/microsoft-edge-%E3%81%AE%E9%96%B2%E8%A6%A7%E5%B1%A5%E6%AD%B4%E3%82%92%E8%A1%A8%E7%A4%BA%E3%81%BE%E3%81%9F%E3%81%AF%E5%89%8A%E9%99%A4%E3%81%99%E3%82%8B-00cf7943-a9e1-975a-a33d-ac10ce454ca4) や [InPrivate ブラウズ](https://support.microsoft.com/ja-jp/microsoft-edge/microsoft-edge-%E3%81%A7-inprivate-%E3%83%96%E3%83%A9%E3%82%A6%E3%82%BA%E3%82%92%E4%BD%BF%E3%81%86-e6f47704-340c-7d4f-b00d-d0cf35aa1fcc) により改善するか
- 別ユーザーでも事象が発生するか
- 同じユーザーで、別 PC でも事象が発生するか
- 再現頻度（100% 発生するか、時々なのか）

## 業務影響、達成事項、背景やスケジュール

発生している問題が業務やプロジェクト、またそのスケジュールへ与える具体的な影響、問題を解消することで達成すべき状態や、達成すべき理由につきまして、ご提供くださいますと幸いです。
お客様個別の事情を勘案し、より適切なご案内を差し上げるため、これらの情報を伺うことがございます。

## サポート インスタンスについて

サポート インスタンスへお客様の事象が発生しているインスタンスをコピーしていただくことで、事象の再現と調査を一貫して行うことが可能となり、早期解決が見込めます。 サポート インスタンスは、サポート チームが調査などに必要と判断した場合に作成するため、お客様のご要望で作成することはできませんが、お問合せ起票時に下記の対応を実施いただけますと迅速に作成することができます。

- サポート インスタンスの作成に同意いただける場合は、起票時に作成同意の旨を記載ください
- サポート インスタンスの作成に社内 / エンド顧客の同意が必要な場合は、事前にご確認をお願いいたします

サポート インスタンスの詳細につきましては [サポート インスタンスの提供](https://jpdynamicscrm.github.io/blog/powerplatform/Provide-Support-Instance/) をご参照ください。


## 仕様の確認に関する調査について

Dynamics 365 の動作について、仕様の確認をお問い合わせいただく場合がありますが、Dynamics 365 では様々な修正やお客様からの機能実装などのご要望に応じて継続的に内部コンポーネントを更新していることから、個々のテナント環境での動作差異を含め、Dynamics 365 サービスの説明をはじめ弊社サイトに記載の内容以上の仕様に関する情報のご提供が困難な場合がございます。

原則としては公開されている情報以上の仕様についての情報は提供しておりませんが、ご質問の背景をお知らせいただくことで、代替となる手法など参考情報のご案内が可能になる場合がございます。

## カスタマイズにより問題が発生している場合

弊社が提供する API が文書通りに機能しない場合や、API 利用により製品機能に意図しない影響を及ぼす場合などは、発生事象についての詳細説明、再現可能な最小のスクリプトのコピーと再現手順をご提供ください。

お客様様がご利用のスクリプトをそのままご提供される場合、発生事象と無関係なコードを含みますため、調査が困難となります。まずは製品の意図しない動作(**の情報が取得できるはずが取得されてこない)を引き起こしているお客様のスクリプトの箇所を切り分け、スクリプトを簡略化ください。

「スクリプトを変更していないが意図しない動作が発生している」旨のお問い合わせをいただくことがございますが、その場合であっても、まずはお客様にて、発生事象に対してスクリプトの切り分けや簡素化をご対応くださいますようお願いいたします。

[カスタム スクリプトを簡略化する](https://learn.microsoft.com/ja-jp/troubleshoot/power-platform/power-apps/isolate-model-app-issues#simplify-custom-scripts) も併せてご参照くださいますと幸いです。


## 参考

以下の記事もあわせてご確認ください。

- [根本原因分析 (RCA) を要求するにはどのサポート プランが必要ですか。](https://learn.microsoft.com/ja-jp/power-platform/admin/support-overview#which-support-plan-do-i-need-in-order-to-request-a-root-cause-analysis-rca)
- [一般的な Power Apps デバッグ戦略](https://learn.microsoft.com/ja-jp/troubleshoot/power-platform/power-apps/isolate-common-issues)
- [クラウド サポートをご利用いただく際の留意点](https://jpdynamicscrm.github.io/blog/powerplatform/Notes-when-using-support.md)
