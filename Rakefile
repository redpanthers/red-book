task :entry do
  info = get_info(section_id: 'Section ID (intro)', section_class: 'Section Class (h1)', title: 'title (Introduction)', number: 'Priority number (eg: 1000)')

  text = "---
sectionid: #{info[:section_id]}
sectionclass: #{info[:section_class]}
title: #{info[:title]}
number: #{info[:number]}
---

"

  filename = "#{info[:number]}-#{info[:section_id]}.md"
  path = File.join('_entries', filename)
  File.open(path, 'w') { |f| f << text }
end

def get_info(qns)
  qns.map { |k, qn|
    [k, ask("#{qn}: ")]
  }.to_h
end

def ask(qn)
  STDOUT.print qn
  STDIN.gets.chomp
end