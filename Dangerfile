declared_trivial = github.pr_title.include? "#trivial"


warn("PR is classed as Work in Progress") if github.pr_title.include? "WIP"


warn("とてつもなくでかいPRだね。もっとスリムにできない？") if git.lines_of_code > 50

message('プルリクありがとね。でもマージするかわからないよ？')

warn('あぶねぇあぶねぇ')

fail('ドキュメント書いてないでしょ？')


fail("fdescribe left in tests") if `grep -r fdescribe specs/ `.length > 1
fail("fit left in tests") if `grep -r fit specs/ `.length > 1

if !git.modified_files.include?("README.md") && has_app_changes
  message "本当にいいんだな？"
end