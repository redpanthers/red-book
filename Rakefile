task :entry do
  info = get_info(section_id: 'unique ID (intro)',
                          section_class: 'Section Class (h1)',
                          title: 'title (Introduction)', 
                          is_parent: 'Is parent? Y/N',
                          parent_id: 'Parent id (eg: intro)',
                          number: 'Priority number (eg: 1000)')

  text = "---
sectionid: #{info[:section_id]}
sectionclass: #{info[:section_class]}
title: #{info[:title]}
"

  if info[:is_parent].downcase == 'y'
    text = text + "is-parent: true
"
  end

  if info[:parent_id] != ""
    text = text + "parent-id: #{info[:parent_id]}
"
  end
  text = text +"number: #{info[:number]}
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